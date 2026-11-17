# Exports for YOYABA, pulled 31 October 2026

Hi, Jan here (Sales Ops). Anna asked me to pull everything we have. I did not have time to clean much, sorry. Notes per file, as far as I know.

## HubSpot
- hubspot_contacts_export.csv: all contacts. became_mql_date is when they became an MQL. contact_owner is the current owner.
- hubspot_contact_attribution_export.csv: the source drill-downs, first page seen and UTM fields for the same contacts. The main export timed out with those columns in it, so they are a separate file.
- hubspot_contact_property_history.csv: change history for lifecycle stage, contact owner and lead status. Mia set this up for an audit last year, I just exported it.
- hubspot_companies_export.csv: all companies. I removed the duplicates from the Pipedrive migration (I think all of them).
- hubspot_deals_export.csv: all deals, both pipelines. Amounts are in EUR.
- hubspot_deal_stage_history.csv: when each deal entered each stage.
- hubspot_workflows.csv: the list from Automation > Workflows.
- outreach_activity_log.csv: SDR emails and calls from Outreach. hubspot_sequence_activity.csv is the same thing for the few people who use HubSpot Sequences instead.
- deal_loss_notes.csv: the closed lost note field. Not every rep fills it in.
- gong_call_summaries.csv: Gong's AI summaries, for calls that are linked to a deal.

## Reporting
- board_deck_funnel_export.csv: the numbers from the Looker dashboard that goes into the board deck.
- looker_forecast_snapshot_2026-07-01.csv: the deals in the Q3 forecast as Anna saw them on 1 July.

## Other systems
- stripe_subscriptions.csv: self-serve customers. These are not in HubSpot as customers (the sync is off).
- finance_arr_by_motion_monthly.csv: Martin's ARR sheet. It never matches HubSpot. Martin says HubSpot is wrong.
- google_ads_*, linkedin_ads_*: from Clara in marketing and the paid agency. The ad exports start in January 2025. Performance Max does not report search terms. The LinkedIn demographics file covers January to October 2026 only and leaves out small segments.
- search_console_*, ai_search_*, ahrefs_domain_overview_monthly.csv, website_content_inventory.csv, website_traffic_daily.csv: from the website team. The Search Console query file is only the 12 queries they track by hand.
- marketing_events.csv, g2_reviews.csv, productboard_top_requests.csv, gtm_team_roster.csv, gtm_tool_licenses.csv: various.

## Things I know are off
- Segment values are a mess (MM, Mid-Market, mid market and so on).
- Some deals have no deal type. I think those are the old Pipedrive ones.
- Some deal owners have left the company.
