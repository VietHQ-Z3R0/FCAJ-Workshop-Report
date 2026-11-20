---
title: "Blog 3"
date: 2026-11-05
weight: 3
chapter: false
pre: " <b> 3.3. </b> "
---

# AURORA SERVERLESS V2: AUTOMATIC PAUSE AND RESUME FOR DATABASE COST OPTIMIZATION

## Overview

Some applications use their databases heavily during business hours but have long periods of low activity outside those hours. With a database configuration that continuously maintains compute capacity, this pattern can lead to costs that do not closely match actual demand.

Amazon Aurora Serverless v2 can automatically scale database capacity based on workload. For supported Aurora engine versions, it can also scale down to **0 Aurora Capacity Units (ACUs)** and automatically pause after a configured period without user-initiated activity. When a new connection request arrives, the database can automatically resume.

## Key points to know

* Aurora Serverless v2 capacity is measured in ACUs. Each ACU represents a combination of processing and memory capacity.
* To use automatic pause, configure the cluster's minimum capacity to **0 ACUs** and set the idle period before pausing.
* When an eligible instance has no user-initiated connections for the configured period, it can automatically pause; a subsequent connection request can trigger resume.
* Instance-capacity charges are not incurred while an instance is paused. Other database charges, such as storage, should still be considered when estimating total cost.
* Automatic pause is available only for supported Aurora PostgreSQL and Aurora MySQL engine versions and configurations. Check the current compatibility and limitations before enabling it.
* Applications should tolerate a delay while a paused instance resumes. AWS notes that a typical resume for a small number of incoming connections can take approximately 15 seconds.

## Example use case

Consider a development or internal application that is used mainly during the morning and receives very little traffic overnight. With Aurora Serverless v2 configured for a minimum capacity of 0 ACUs, an eligible database instance can pause after the configured inactivity period. When users return and the application opens a database connection, the instance resumes and begins serving requests again.

This can reduce compute-capacity costs during extended idle periods without requiring an operator to manually stop and start the database every day. It is most appropriate for workloads that can tolerate the resume delay and do not require uninterrupted low-latency database access.

## Important considerations

Automatic pause does not happen simply because an application sends no SQL statements. Open user-initiated connections can prevent an instance from pausing, and some features or cluster configurations can affect eligibility. Confirm that the engine version supports 0 ACUs, review the documented limitations, and test connection retry and timeout behavior. CloudWatch metrics such as `ServerlessDatabaseCapacity` can help verify whether the instance has reached zero capacity.

## Image

<!-- Add the Aurora Serverless v2 architecture diagram or a screenshot of the minimum-capacity and auto-pause settings here. -->

## Link

<!-- Paste the Facebook AWS Study Group post URL here. -->

## Guide

* [Scaling to zero ACUs with automatic pause and resume](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2-auto-pause.html)
* [How Aurora Serverless v2 works](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2.how-it-works.html)
