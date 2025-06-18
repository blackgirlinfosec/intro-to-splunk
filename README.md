# Getting Started with Splunk: Exploring the Basics

## 🧠 Why I'm Doing This

As I prepare for the job search, I’ve been researching the tools that show up most in SOC analyst job descriptions. One name that comes up over and over again is Splunk. From my research, It's one of the most widely used SIEMs in the industry, and I wanted to understand it for myself—not just in theory, but in practice.

This lab is my first hands-on experience inside the Splunk Cloud platform. I created it out of curiosity and a genuine interest in getting more comfortable with tools I know I’ll need on the job.

## 💻 What I Did

I signed up for a free Splunk Cloud trial and explored the built-in logs using the `Search & Reporting` app. I didn’t upload any custom data for this lab. Instead, I worked with Splunk’s own internal logs (`index=_internal`) to get a feel for how the platform works.

Here’s what I explored:

- Navigated the Splunk Cloud dashboard and Search app
- Searched Splunk’s internal logs using `index=_internal`
- Ran my first SPL pipeline using `stats count`
- Identified the most common sourcetypes with `top sourcetype`
- Viewed log severity levels with `top log_level`
- Filtered logs where `log_level=ERROR`
- Opened the Visualization tab to try a pie chart

## 🔍 SPL Commands I Practiced

```spl
index=_internal
index=_internal | stats count
index=_internal | top sourcetype
index=_internal | top log_level
index=_internal log_level=ERROR
```
## 📸 Screenshots
- splunk_cloud_dashboard_home.png — initial login landing page
- splunk_search_dashboard_empty.png — inside the Search & Reporting app before running a query
- splunk_internal_search_results.png — results from index=_internal
- splunk_stats_count_internal.png — total number of logs using stats count
- splunk_top_sourcetypes.png — identifying common sourcetypes
- splunk_top_log_levels.png — viewing log levels like INFO, WARN, ERROR

## 🧠 What I Learned
This lab helped me build a basic level of comfort using Splunk Cloud. I now understand how to navigate the interface, run a search, and analyze logs using SPL. Commands like stats count and top sourcetype helped me begin looking at patterns in the data.

Even though I didn’t upload custom logs or build dashboards yet, this was a strong introduction. I got hands-on practice that goes beyond theory, and I feel more confident stepping into a tool I know I’ll be using as a SOC analyst.

