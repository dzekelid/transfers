swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metarouter/rest/routeservice/v2/route.json:
    get:
      summary: Avoid Transit Routes Involving Transfers
      description: "*Request a direct public transit route excluding changes and transfers*\n\nPublic
        transit routes can be requested using the `metarouter/rest/routeservice/v2/route.json`
        endpoint. The `changes `parameter is used to indicate the number of changes
        or transfers desired. \n\n\n\n* **startX**  `number`\n \\- The longitude of
        the start point of your journey.    e.g. `13.377`\n\n* **startY**  `number`\n
        \\- The latitude of the start point of your journey.    e.g. `52.515`\n\n*
        **destX**  `number`\n \\- The longitude of the destination point of your journey.
        \   e.g. `13.377`\n\n* **destY**  `number`\n \\- The latitude of the destination
        point of your journey.    e.g. `52.515`\n\n* **time**  `text`\n \\- Time in
        format `yyyy-mm-ddThh:mm:ss`.\n\n* **app_id**  `text`\n \\- A 20 bytes Base64
        URL-safe encoded string used for the authentication of the client application.
        \   You must include an app_code and app_code with every request.\n\n* **app_code**
        \ `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an app_code and app_code with
        every request.\n\n* **routing**  `enum`\n \\- Type of routing response required.
        \ tt: time-table routing, i.e. route response will show scheduled arrival/departure
        times of the transit at the stations.  sr: simple (or estimated) routing,
        i.e. route response will only show \nthe transit journey but without scheduled
        arrival/departure times.  all: for both estimated and time-table routing.
        \ Default: tt  \n\n    Valid values are : `tt`, `sr`, `all`\n\n* **changes**
        \ `enum`\n \\- Maximum number of changes or transfers. \n                Valid
        values: 0-6 or -1. Default: -1 (any number of transfers permitted).\n\n    >**NOTE:**
        In areas where this parameter is not supported the route response will show
        an attribute `sup_changes=0` in the `Connections` node.\n\n    Valid values
        are : `-1`, `0`, `1`, `2`, `3`, `4`, `5`, `6`"
      operationId: MetarouterRestRouteserviceV2RouteJsonGet8
      x-api-path-slug: metarouterrestrouteservicev2route-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: changes
      - in: query
        name: destX
      - in: query
        name: destY
      - in: query
        name: routing
      - in: query
        name: startX
      - in: query
        name: startY
      - in: query
        name: time
      responses:
        200:
          description: OK
      tags:
      - Avoid
      - Transit
      - Routes
      - Involving
      - Transfers