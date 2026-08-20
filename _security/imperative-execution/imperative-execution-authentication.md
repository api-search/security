---
api_key_in: []
api_specs:
- filename: imperative-execution-iqx-asyncapi.yml
  format: yaml
  label: IntelligentCross IQX Market Data Feed
  slug: intelligentcross-iqx-market-data-feed
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperative-execution/refs/heads/main/asyncapi/imperative-execution-iqx-asyncapi.yml
auth_types:
- none-public
- network-access-control
- contractual-eligibility
description: ''
kind: authentication
layout: security
method: searched
name: Imperative Execution Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imperative Execution secures its APIs with none-public, network-access-control, and contractual-eligibility across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imperative Execution
provider_slug: imperative-execution
scheme_count: 4
schemes:
- applies_to: IntelligentCross FIX Order Entry API
  description: IntelligentCross only permits registered US broker-dealers to be subscribers. A subscriber must be in good standing with a self-regulatory organization and satisfy additional eligibility requirements before connectivity is provisioned.
  name: subscriber-eligibility
  onboarding_contact: ops@intelligentcross.com
  source: https://www.imperativex.com/faq
  type: contractual
- applies_to:
  - IntelligentCross FIX Order Entry API
  - IntelligentCross IQX Market Data Feed
  description: Subscribers connect to the ATS from a specified internet protocol address over FIX, reaching primary matching engines in the Equinix NY4 data center via NY4 cross-connects or a network service provider with an NY4 presence. Pico is the venue's co-location and network provider. There is no public internet endpoint for either surface.
  name: network-access-control
  source: https://www.imperativex.com/faq
  type: network
- applies_to: IntelligentCross FIX Order Entry API
  description: Order-entry identity is asserted on each message through the FIX fields the ATS requires - notably ClientID and the subscriber's Broker MPID, which are also the keys the venue's anti-internalization (self-match prevention) control is enforced by. Book selection is asserted with ExDestination (tag 100). The full FIX specification is released to subscribers on request and is not public.
  name: fix-session-and-order-identity
  protocol: FIX 4.2
  source: https://www.imperativex.com/faq
  spec_availability: subscriber-only, on request from ops@intelligentcross.com
  type: protocol
- applies_to: IntelligentCross IQX Market Data Feed
  description: The IQX feed is disseminated over multicast UDP inside the venue's connectivity footprint and carries no per-consumer authentication. Reachability is the access control. IntelligentCross does not charge for market data through IQX. The specification, the daily symbol mapping file and sample PCAP captures are published openly over HTTPS with no credential.
  name: multicast-subscription
  source: http://iqx.imperativex.com/IntelligentCrossMarketDataFeedSpec.v.1.11.pdf
  type: none
slug: imperative-execution-authentication
source_filename: imperative-execution-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://www.imperativex.com/faq\ndocs: https://www.imperativex.com/faq\nsummary:\n  types: [none-public, network-access-control, contractual-eligibility]\n  api_key_in: []\n  oauth2_flows: []\n  note: 'IntelligentCross publishes no public credential-based authentication scheme -\n    there is no API key, OAuth or OIDC surface, because neither of its interfaces is an\n    HTTP API. Access is controlled contractually (registered US broker-dealer subscribers\n    only) and at the network layer (private cross-connects into Equinix NY4). Identity on\n    the wire is carried by FIX session and order-level identifiers rather than a bearer\n    credential.'\nschemes:\n- name: subscriber-eligibility\n  type: contractual\n  applies_to: IntelligentCross FIX Order Entry API\n  description: IntelligentCross only permits registered US broker-dealers to be subscribers.\n    A subscriber must be in good standing with a self-regulatory organization\
  \ and satisfy\n    additional eligibility requirements before connectivity is provisioned.\n  onboarding_contact: ops@intelligentcross.com\n  source: https://www.imperativex.com/faq\n- name: network-access-control\n  type: network\n  applies_to: [IntelligentCross FIX Order Entry API, IntelligentCross IQX Market Data Feed]\n  description: Subscribers connect to the ATS from a specified internet protocol address\n    over FIX, reaching primary matching engines in the Equinix NY4 data center via NY4\n    cross-connects or a network service provider with an NY4 presence. Pico is the venue's\n    co-location and network provider. There is no public internet endpoint for either\n    surface.\n  source: https://www.imperativex.com/faq\n- name: fix-session-and-order-identity\n  type: protocol\n  applies_to: IntelligentCross FIX Order Entry API\n  protocol: FIX 4.2\n  description: Order-entry identity is asserted on each message through the FIX fields the\n    ATS requires - notably ClientID and\
  \ the subscriber's Broker MPID, which are also the\n    keys the venue's anti-internalization (self-match prevention) control is enforced by.\n    Book selection is asserted with ExDestination (tag 100). The full FIX specification is\n    released to subscribers on request and is not public.\n  spec_availability: subscriber-only, on request from ops@intelligentcross.com\n  source: https://www.imperativex.com/faq\n- name: multicast-subscription\n  type: none\n  applies_to: IntelligentCross IQX Market Data Feed\n  description: The IQX feed is disseminated over multicast UDP inside the venue's connectivity\n    footprint and carries no per-consumer authentication. Reachability is the access control.\n    IntelligentCross does not charge for market data through IQX. The specification, the\n    daily symbol mapping file and sample PCAP captures are published openly over HTTPS with\n    no credential.\n  source: http://iqx.imperativex.com/IntelligentCrossMarketDataFeedSpec.v.1.11.pdf\npublic_unauthenticated_resources:\n\
  - url: https://s3.amazonaws.com/iqx.imperativex.com/Symbol-Mapping.txt\n  http_status: 200\n- url: https://s3.amazonaws.com/iqx.imperativex.com/20230103-IQX-mdA.pcap.gz\n  http_status: 200\n- url: http://iqx.imperativex.com/IntelligentCrossMarketDataFeedSpec.v.1.11.pdf\n  http_status: 200\nnot_present:\n  oauth2: true\n  openid_connect: true\n  api_keys: true\n  mutual_tls_documented: true\n  note: Probed for /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    on imperativex.com and www.imperativex.com - both 404. See well-known/imperative-execution-well-known.yml.\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://www.imperativex.com/faq\n  http_status: 200\n- fetched: '2026-08-04'\n  url: http://iqx.imperativex.com/IntelligentCrossMarketDataFeedSpec.v.1.11.pdf\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperative-execution/refs/heads/main/authentication/imperative-execution-authentication.yml
summary_line: none-public/network-access-control/contractual-eligibility · 4 schemes
tags:
- Company
- Financial-Services
- Capital Markets
- Trading
- Market Data
- Equities
- Alternative Trading System
- FIX Protocol
- Multicast Market Data
- Fintech
---
