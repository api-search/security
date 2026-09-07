---
anonymous_access: false
api_key_in: []
auth_types: []
description: Zendrive's public integration surface is a mobile SDK, and its authentication model is an application key (also called the SDK key) carried in ZendriveConfiguration and validated against Zendrive's servers during +[Zendrive setupWithConfiguration:delegate:completionHandler:]. There is no OAuth surface, no OpenID Connect discovery document, and no publicly reachable token endpoint — every /.well-known/openid-configuration and /.well-known/oauth-authorization-server probe on every known Zendrive host missed (see well-known/zendrive-well-known.yml). The server-side Analytics REST API used a separate credential documented at docs.zendrive.com, which is now a dangling Cloudflare CNAME, so that scheme cannot be captured first-hand and is deliberately not described here.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zendrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zendrive declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zendrive
provider_slug: zendrive
scheme_count: 2
schemes:
- description: '"Your application key. Pass in the application key for your app." REQUIRED, must be a valid non-nil string; validated with +[Zendrive isValidInputParameter:]. Setup requires a network connection because the key is validated server-side, and returns kZendriveErrorInvalidSDKKeyString (0) when the key is rejected and kZendriveErrorNetworkUnreachable (1) when validation cannot reach the server.'
  in: sdk-configuration
  issuance:
    documented_url: https://developers.zendrive.com/signup
    note: The SDK reference still instructs developers to create a key at https://developers.zendrive.com/signup. That host has no DNS record; the sample-app READMEs point at https://app.zendrive.com/signup, which is also NXDOMAIN. New keys can no longer be obtained, so this is a DEAD issuance path and is not wired as a SignUp pointer.
    status: 0
  label: Zendrive application key (SDK key)
  name: applicationKey
  required: true
  type: apiKey
- description: '"Unique ID for the current user. This can be any ID used by your app to identify its users. This is the ID which will be used in Zendrive reports." REQUIRED alongside the application key; changing it mid-session is equivalent to teardown followed by a fresh setup.'
  in: sdk-configuration
  label: Driver identifier
  name: driverId
  note: Not a credential — it is the tenant-scoped subject the application key authorizes. Recorded because setup fails without it.
  required: true
  type: identifier
slug: zendrive-authentication
source_filename: zendrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://zendrive-root.bitbucket.io/ios/docs/latest/Classes/ZendriveConfiguration.html ;\n  https://zendrive-root.bitbucket.io/ios/docs/latest/Classes/Zendrive.html\nname: Zendrive authentication\ndescription: >-\n  Zendrive's public integration surface is a mobile SDK, and its authentication model is an\n  application key (also called the SDK key) carried in ZendriveConfiguration and validated\n  against Zendrive's servers during +[Zendrive setupWithConfiguration:delegate:completionHandler:].\n  There is no OAuth surface, no OpenID Connect discovery document, and no publicly reachable\n  token endpoint — every /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  probe on every known Zendrive host missed (see well-known/zendrive-well-known.yml). The\n  server-side Analytics REST API used a separate credential documented at docs.zendrive.com,\n  which is now a dangling Cloudflare CNAME, so that\
  \ scheme cannot be captured first-hand and\n  is deliberately not described here.\nsurface: mobile-sdk\nschemes:\n- type: apiKey\n  name: applicationKey\n  label: Zendrive application key (SDK key)\n  in: sdk-configuration\n  required: true\n  description: >-\n    \"Your application key. Pass in the application key for your app.\" REQUIRED, must be a\n    valid non-nil string; validated with +[Zendrive isValidInputParameter:]. Setup requires a\n    network connection because the key is validated server-side, and returns\n    kZendriveErrorInvalidSDKKeyString (0) when the key is rejected and\n    kZendriveErrorNetworkUnreachable (1) when validation cannot reach the server.\n  issuance:\n    documented_url: https://developers.zendrive.com/signup\n    status: 0\n    note: >-\n      The SDK reference still instructs developers to create a key at\n      https://developers.zendrive.com/signup. That host has no DNS record; the sample-app\n      READMEs point at https://app.zendrive.com/signup,\
  \ which is also NXDOMAIN. New keys can\n      no longer be obtained, so this is a DEAD issuance path and is not wired as a SignUp\n      pointer.\n- type: identifier\n  name: driverId\n  label: Driver identifier\n  in: sdk-configuration\n  required: true\n  description: >-\n    \"Unique ID for the current user. This can be any ID used by your app to identify its\n    users. This is the ID which will be used in Zendrive reports.\" REQUIRED alongside the\n    application key; changing it mid-session is equivalent to teardown followed by a fresh\n    setup.\n  note: >-\n    Not a credential — it is the tenant-scoped subject the application key authorizes. Recorded\n    because setup fails without it.\nsession:\n  setup: +[Zendrive setupWithConfiguration:delegate:completionHandler:]\n  teardown: +[Zendrive teardown...]\n  wipe: +[Zendrive wipeOut:]\n  note: >-\n    Credentials are established once at setup. Changing applicationKey or driverId across\n    repeated setups behaves as teardown-then-setup.\
  \ The data region cannot be changed after\n    setup without calling wipeOut first (kZendriveErrorUnauthorizedRegionSwitch, 110).\ndata_residency:\n  parameter: ZendriveConfiguration.region\n  values:\n  - id: ZendriveRegionUS\n    value: 0\n    description: User's data will reside in the US region. This is the default.\n  - id: ZendriveRegionEU\n    value: 1\n    description: User's data will reside in the EU region.\n  reference: https://zendrive-root.bitbucket.io/ios/docs/latest/Enums/ZendriveRegion.html\n  note: >-\n    Region is per-application and enforced at setup. An application not provisioned for a\n    region receives kZendriveErrorRegionUnsupported (109).\ndeprovisioning:\n  error: kZendriveErrorUserDeprovisioned (111)\n  description: User is not authorized to use this application.\ngaps:\n- No OAuth 2.0 or OIDC surface is published.\n- No scopes/ artifact is applicable — the model is a single opaque application key, not a scoped grant.\n- >-\n  The Analytics REST API credential\
  \ model (docs.zendrive.com/en/latest/api/) is unrecoverable:\n  every host that served it is NXDOMAIN or a dangling CNAME.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendrive/refs/heads/main/authentication/zendrive-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Telematics
- Mobility
- Insurance
- Automotive
- Fleet Management
- Driving Behavior
- Mobile SDK
- Risk
- Acquired
---
