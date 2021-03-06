# Managing and Configuring Apps [](id=managing-and-configuring-apps)

There are two places in the Control Panel where you can manage and configure 
apps: the App Manager, and the Components listing. The App Manager lets you 
manage apps in Liferay's OSGi framework. You can use the App Manager to install, 
activate, deactivate, and delete apps in your Liferay instance. You can manage 
apps at the app suite, app, and OSGi module levels. 

Unlike the App Manager, the Components listing lets you view and manage apps 
regardless of Liferay's OSGi framework. The Components listing also differs by 
letting you view apps by type (portlet, theme, and layout template), and set app 
permissions. Although the Components listing lets you activate and deactivate 
apps, you can't use it to install or delete apps. 

First, you'll learn how to use the App Manager.

## Using the App Manager [](id=using-the-app-manager)

Access the App Manager by selecting *Control Panel* &rarr; *Apps* &rarr; *App 
Manager*. The App Manager lists your Liferay instance's app suites and apps in 
separate tables. The bar above the first table lets you display the contents of 
both by category and status. You can also sort the tables by title. Click the up 
or down arrows to perform an ascending or descending sort, respectively. To 
search for an app suite, app, or module, use the search bar at the top-right. 
This is often the quickest way to find exactly what you're looking for. 

![Figure 1: The App Manager lets you manage the app suites and apps installed in your Liferay instance.](../../images/app-manager.png)

Each item listed in the tables contains a description (if available), version, 
and status. The status refers to the item's OSGi status:

- Installed: The item is installed in the OSGi framework. 
- Resolved: The item's dependencies have been resolved by the OSGi framework. 
  Resolved items can typically be activated. Note, however, that some items, 
  like WSDD modules containing SOAP web services, can't be activated and are 
  intended to remain in the Resolved state.
- Active: The item is running in the OSGi framework. 

Clicking the Actions button (![Actions](../../images/icon-actions.png)) to each 
item's right brings up a menu that lets you activate, deactivate, or delete the 
item. 

To view an item's contents, click its name in the table. If you click an app 
suite, a new table lists the suite's apps. If you click an app, a new table 
lists the app's modules. If you click a module, a new table lists the module's 
components. The component level is as far down as you can go in OSGi without 
getting into the source code. After that, it's turtles all the way down. At any 
level in the App Manager, you can use the link trail above the table to go back 
in the hierarchy. 

For information on using the App Manager to install an app, see the article 
[Installing Apps Manually](/discover/portal/-/knowledge_base/7-0/installing-apps-manually). 

Next, you'll learn how to use the Components listing. 

## Using the Components Listing [](id=using-the-components-listing)

Access the Components listing by selecting *Control Panel* &rarr; 
*Configuration* &rarr; *Components*. The Components listing first shows a table 
containing a list of portlets installed in your Liferay instance. Select the 
type of component to view--portlets, themes, or layout templates--by clicking 
the matching tab on top of the table. To configure a component, select its name 
in the table, or select *Edit* from its Actions button (![Actions](../../images/icon-actions.png)). 
Doing either opens the same configuration screen. 

![Figure 2: The Components listing lets you manage the portlets, themes, and layout templates installed in your Liferay instance.](../../images/components-list.png)

The configuration screen lets you view a component's module ID and plugin ID, 
activate or deactivate the component, and change the component's Add to Page 
permission. The component's module ID and plugin ID appear at the top of the 
screen. You can activate or deactivate a component by checking or unchecking the 
*Active* checkbox, respectively. To change a component's Add to Page permission 
for a role, select the role's *Change* button in the permissions table. This 
takes you to *Control Panel* &rarr; *Users* &rarr; *Roles*, where you can change 
the component's permissions for the selected role. 

![Figure 3: You can also activate or deactivate a component, and change its permissions.](../../images/components-configuration.png)

Awesome! Now you know how to manage the apps installed in your Liferay 
instances. 
