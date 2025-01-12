docker run --name joon -e MYSQL_ROOT_PASSWORD=root -d mysql:latest

- differences
    - no granularity in error responses
    - jwt replaced with cached uuids
    - /api/user/address/create new address not returned
    - /api/user/address/update new address not returned
    - no auth guard in order controllers
    - responses wrapped

- missing features
    - ignoring set headers middleware
    - jwt - replaced with uuid tokens and redis

- hard in code but easy in ui:
    - nested resolvables

- hard in ui easy in code:
    - jq nesting

- hard in both:
    - getting parameters names (saved in store, req, etc)

- removing dbDump

- apis done
    - /api/area/areas: OK
    - /api/customer-authentication: OK
    - /api/customer-registration: OK
    - /api/partner-authentication: OK
    - /api/partner-registration: OK
    - /api/bundles: OK
    - /api/service/specialOffer: OK
    - /api/service/trending: OK
    - /api/category/all OK
    - /api/category/all/salon OK
    - /api/category/all/spa OK
    - /api/city/cities: OK
    - /api/favorite/create: OK
    - /api/favorite/delete: OK
    - /api/favorite/get foreach
    - /api/lead/create: OK
    - /api/notification/get: OK
    - /api/order/status-change: TESTED WITH ORDER ID 7 - NOTIFICATION WORKING WITH 401 (NEED FCM)
    - /api/order/customer-orders OK
    - /api/order/partner-orders OK
    - /api/rates: OK
    - /api/user/address/create: OK
    - /api/user/address/customer-addresses: OK
    - /api/user/address/is_default: OK
    - /api/user/address/update: OK
    - /api/user/details/update: OK
    - /api/user/address/delete: NOT TESTED - CURRENTLY USING HARD DELETE