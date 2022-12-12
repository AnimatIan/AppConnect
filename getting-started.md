---

copyright:
  years: 2017, 2021
lastupdated: "2021-11-12"

keywords: app connect, integration, application, getting started

subcollection: AppConnect

content-type: tutorial
account-plan: lite
completion-time: 10m

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}
{:step: data-tutorial-type='step'}


# Getting started with {{site.data.keyword.appconnect_notm}}
{: #getting-started}
{: toc-content-type="tutorial"}
{: toc-completion-time="10m"}

{: #deprecation}
Service plans for {{site.data.keyword.appconservicefull}} have been deprecated, and any instances of {{site.data.keyword.appconnect_notm}} plans that still exist on 30 November 2023 will be deleted. To continue using IBM App Connect, you should migrate to an alternative provision. For more information, see [Deprecation of IBM App Connect on IBM Cloud service plans](deprecation_of_ibm_cloud_foundry.md) {: deprecated}

In this getting started tutorial, we'll take you through how to use {{site.data.keyword.appconservicefull}} to create an event driven flow that will take you about 10 minutes to implement.
{: shortdesc}

As the name suggests, an event-driven flow consists of an event in a source application, which triggers the flow, and one or more actions in target applications. So when something happens in the source application, an action is triggered in your target applications. To create an event-driven flow that connects your cloud-based applications, complete the following steps.

## Before you begin
{: #gs-prereqs}

Create an instance of the {{site.data.keyword.appconserviceshort}} service, to launch {{site.data.keyword.appconnect_notm}}.

## Create an event-driven flow
{: #create-flow}
{: step}

1.  On the {{site.data.keyword.appconnect_notm}} dashboard, click **New** > **Event-driven flow**.
    {{site.data.keyword.appconnect_notm}} saves your changes automatically as you go. If you navigate away from the flow at any stage, the flow is saved as a draft flow that you can complete at another time.
1.  Enter a name for your flow.

## Select a trigger
{: #select-trigger}
{: step}

1.  Select the trigger event to start your flow by expanding an application and selecting an event.
1.  If you're not already connected to your application, click **Connect** and enter your login details for the application.
    You might have to provide extra connection details for some applications; if you need help with finding credentials for a particular application, see the [How-to guides for apps ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=designer-how-guides-apps).

## Select an action
{: #select-action}
{: step}

1.  Select the action to be triggered in your second application by clicking the plus icon in the flow ![Add an application icon](/images/AddApp.jpg), expanding an application, and selecting an action. If necessary, click **Connect** and enter your login details for the target application.
1. Enter the data that you want to transfer between your applications. You can add source field names manually by clicking in a field then clicking the mapping icon ![Mapping icon](/images/MappingIcon.jpg). You can also type in text, or use a transformation function to customize the source value. For more information, see [Applying JSONata functions to transform your data ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=actions-applying-jsonata-functions-transform-your-data).

## Refine your flow
{: #refine-flow}
{: step}

Optional: You can refine how your flow works by doing the following things:
- Add more target applications and actions by clicking the plus icon in the flow ![Add an application icon](/images/AddApp.jpg).
- Add retrieval actions to your flow to retrieve items that match certain criteria or retrieve a specified number of records.  You can also add retrieval actions that define error handling or define how you handle the items that are retrieved (see [Using App Connect to retrieve items from your applications ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=connect-retrieving-items-from-your-applications)).
- Add some conditional logic to perform different actions that depend on the data that is received from applications in your flow (see [Adding conditional logic to a flow ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=utilities-if-conditional)).

## Start your flow    
{: #start-flow}
{: step}

When your flow is configured, open the options menu on the header bar and click **Start flow**.

## Next steps
{: #gs-next-steps}

If you return to the {{site.data.keyword.appconnect_notm}} dashboard, you can see that your flow is running.  When an event happens in the first application, an action is triggered automatically by {{site.data.keyword.appconnect_notm}} in your second application. You can view the status of your flows on the {{site.data.keyword.appconnect_notm}} dashboard. To view logs for your flows, click the **Logs** icon ![Logs icon](/images/LogsIcon.jpg).

- For more detailed instructions, how-to guides for specific applications, tutorials, and videos, see the full set of documentation at [IBM App Connect ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud).
- For more information about how to create an event-driven flow, see [Creating an event-driven flow ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=connect-creating-event-driven-flow).
- To follow a tutorial for a typical event-driven flow, see [Creating a ServiceNow incident and sending an email when a Wufoo form is submitted ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/docs/en/app-connect/cloud?topic=td-creating-servicenow-incident-sending-email-when-wufoo-form-is-submitted).
