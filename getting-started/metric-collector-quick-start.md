---
description: >-
  Quick Guide for user to set up Monitoring Metric Collectors for Servers over
  Clouds
---

# Metric Collector Quick Start

## How to Set up

Collect monitoring metric data through the following steps:

* [Prerequisites](metric-collector-quick-start.md#prerequisites)
* [Get API Key for SpaceONE Service Account](metric-collector-quick-start.md#get-api-key-for-spaceone-service-account)
* [Register SpaceONE Service Account](metric-collector-quick-start.md#register-spaceone-service-account-ex-metric-collector)
* [Monitoring Metric Information](metric-collector-quick-start.md#monitoring-metric-information) 
* [Collecting Monitoring Metric Type](metric-collector-quick-start.md#collecting-monitoring-metric-type)

## Prerequisites

Monitoring Metric Collector requires SpaceOne Service Account to collect various vendors includes AWS, Google Cloud, Azure, etc.

## Get API Key for SpaceONE Service Account

Before adding Service Account \(SpaceONE\), you need API Key for SpaceONE.

{% hint style="info" %}
**We currently provide API-Key via administrator only.  
Please, contact your domain administrator of SpaceONE If you don't have an API-Key for SpaceONE service account or send an e-mail for more support \(**_**support@spaceone.dev**_**\)**
{% endhint %}

## Register SpaceOne Service Account \(Ex. Metric Collector\)

Register SpaceONE service account, at **Identity** &gt; **Service Account**

Select **SpaceONE** on Service Provider, and then click +**Add** button.

![](../.gitbook/assets/screen-shot-2020-12-30-at-13.16.21.png)

Register SpaceONE Service Account with following steps,

1. Name Service account
2. Set User ID
3. Put Credentials \(API Key info\)

![](../.gitbook/assets/screen-shot-2020-12-30-at-13.27.39.png)

Configure credentials which has obtained from domain administrator after set service account name and user ID.

You will get a three following items as credential inputs

1. _API Key_
2. _API Key ID_
3. _Identity Endpoint_

All those fields are mandatory.

![](../.gitbook/assets/image-81-.png)

{% hint style="info" %}
**DO NOT assign a project for Monitoring Metric collector Service.**

You can SKIP this step.
{% endhint %}

## Monitoring Metric Information

You can check collected monitoring Metric data information at **Inventory** &gt; **Server** list.  
**Note:** **Recommend Monitoring-metric-collector schedule is a once in day.**

![](../.gitbook/assets/screen-shot-2020-12-30-at-13.53.25.png)

Monitoring metric's values will be updated once collector's job has finished.

![](../.gitbook/assets/screen-shot-2020-12-30-at-14.41.37.png)

Check all collected Monitoring data at **"Raw Data"** tab within path of _**Data -&gt; Monitoring**_

## Collecting Monitoring Metric Type

{% hint style="info" %}
Default metric type that collects via **version 1.5.3.**

**Note**: Monitoring Metric Type will keep updating.
{% endhint %}

### Default Metric Stat

| Stat for Metric | Key | Description |
| :---: | :---: | :---: |
| MAX | max | Maximum value per day |
| AVERAGE | avg | Average value per day |

### Collecting Metrics

<table>
  <thead>
    <tr>
      <th style="text-align:left">Collecting Metric Type</th>
      <th style="text-align:left">Metric name / (Unit)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>CPU</b>
      </td>
      <td style="text-align:left">
        <ul>
          <li>utilization (%)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Memory</b>
      </td>
      <td style="text-align:left">
        <ul>
          <li>usage (%)</li>
          <li>total (bytes)</li>
          <li>used (bytes)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Disk</b>
      </td>
      <td style="text-align:left">
        <ul>
          <li>write_iops (counts)</li>
          <li>write_throughput (bytes)</li>
          <li>read_iops (counts)</li>
          <li>read_throughput (bytes)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Network</b>
      </td>
      <td style="text-align:left">
        <ul>
          <li>received_throughput (bytes)</li>
          <li>received_pps (counts)</li>
          <li>sent_throughput (bytes)</li>
          <li>sent_pps (counts)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

