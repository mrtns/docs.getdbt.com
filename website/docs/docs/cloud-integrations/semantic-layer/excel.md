---
title: "Microsoft Excel"
id: excel
description: "Integrate with Excel to query your metrics in a spreadsheet."
tags: [Semantic Layer]
sidebar_label: "Microsoft Excel"
---

# Microsoft Excel <Lifecycle status='preview'/>

The dbt Semantic Layer offers a seamless integration with Excel Online and Desktop through a custom menu. This add-on allows you to build dbt Semantic Layer queries and return data on your metrics directly within Excel.

## Prerequisites

- You have [configured the dbt Semantic Layer](/docs/use-dbt-semantic-layer/setup-sl) and are using dbt v1.6 or higher.
- You need a Microsoft Excel account with access to install add-ons.
- You have a [dbt Cloud Environment ID](/docs/use-dbt-semantic-layer/setup-sl#set-up-dbt-semantic-layer) and a [service token](/docs/dbt-cloud-apis/service-tokens) to authenticate with from a dbt Cloud account.
- You must have a dbt Cloud Team or Enterprise [account](https://www.getdbt.com/pricing). Suitable for both Multi-tenant and Single-tenant deployment.
  - Single-tenant accounts should contact their account representative for necessary setup and enablement.

import SLCourses from '/snippets/_sl-course.md';

<SLCourses/>


## Installing the add-on

The dbt Semantic Layer Microsoft Excel integration is available to download directly on [Microsoft AppSource](https://appsource.microsoft.com/en-us/marketplace/apps?product=office). You can choose to download this add in for both [Excel Desktop](https://pages.store.office.com/addinsinstallpage.aspx?assetid=WA200007100&rs=en-US&correlationId=4132ecd1-425d-982d-efb4-de94ebc83f26) and [Excel Online](https://pages.store.office.com/addinsinstallpage.aspx?assetid=WA200007100&rs=en-US&correlationid=4132ecd1-425d-982d-efb4-de94ebc83f26&isWac=True)

1. In Excel, authenticate with your host, dbt Cloud environment ID, and service token.
   - Access your Environment ID, Host, and URLs in your dbt Cloud Semantic Layer settings. Generate a service token in the Semantic Layer settings or API tokens settings
   <Lightbox src="/img/docs/dbt-cloud/semantic-layer/sl-and-gsheets.jpg" width="70%" title="Access your Environment ID, Host, and URLs in your dbt Cloud Semantic Layer settings. Generate a service token in the Semantic Layer settings or API tokens settings" />

2. Start querying your metrics using the **Query Builder**. For more info on the menu functions, refer to [Query Builder functions](#query-builder-functions). To cancel a query while running, press the **Cancel** button.

import Tools from '/snippets/_sl-excel-gsheets.md';

<Tools 
type="Microsoft Excel"
bullet_1="There's no timeout limit."
bullet_2="If you're using this extension, make sure you're signed into Microsoft with the same Excel profile you used to set up the Add-In. Log in with one profile at a time as using multiple  profiles at once might cause issues."
/>

<!-- placeholder for excel image URL prop: queryBuilder="/img/docs/dbt-cloud/semantic-layer/sl-and-gsheets.jpg"-->

## FAQs
<FAQ path="Troubleshooting/sl-alpn-error" />
