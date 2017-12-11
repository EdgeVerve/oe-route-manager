# OE Route Manager

The `oe-route-manager` component is a plugin to `oe-studio` which helps managing routes and link between them.

## Navigating to Route Manager

To navigate to route manager, first Go to [oe-designer](http://localhost:3000/designer) and click on the Route Manager icon as marked in the below image:

![Start Page][start-page]

you will be navigated to Route Manager, here left panel will show all the routes available in UIRoutes model in application.

![Route Manager Home][route-manager-home]

Click on routes which needs to be linked, to make them visible in right panel.

![Show Route][show-route]

To add link between two routes click on right side arrow in route block and attach to left side arrow in another route block. It will open a dialogue box where you need to provide event name on which it will navigate to attached route. Click on `CREATE` to create the route.

![Route Config][route-config]

now we will create one more link, which needs to pass payload while navigating to other route.
click on both routes to make visible in right panel.

![Route With Placeholder][route-with-placeholder]

Link these two routes, which will open a new dialogue box shown below.
Dialog box will have input box for event name and for the placeholder which needs to be replaced in route(eg. customerId).
provide the path in payload, from where placeholder value needs to be provided(eg. customer.id)
Click in `CREATE` to create the route.

![Route With Placeholder Config][route-with-placeholder-config]

To save all created routes, click on `Show All` in left panel. It will show all routes available then click on `Save All` to persist the created links.

> Note: Save All button saves only the routes which are visible in workarea.

![Show All Routes][show-all-routes]

## How it works

We create a link between two routes i.e. route1 --> route2, so when element of route1 fire an event that we configured in link it will navigated to route2.

For more info on route navigations click [here](http://evgit/oecloud.io/oecloud-portal/blob/master/guides/route-transitions.md).


[start-page]:  images/designer-home.PNG "Start Page"
[route-manager-home]:  images/route-manager-home.PNG "Route Manager Home"
[show-route]:  images/show-route.PNG "Show Route"
[route-config]:  images/route-config.PNG "Route Config"
[route-with-placeholder]:  images/route-with-placeholder.PNG "Route With Placeholder"
[route-with-placeholder-config]:  images/route-with-placeholder-config.PNG "Route With Placeholder Config"
[show-all-routes]:  images/show-all-routes.PNG "Show All Routes"