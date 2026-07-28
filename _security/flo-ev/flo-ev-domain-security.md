---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flo.com
  spf: true
hosts:
- cert_expires: Oct  6 08:55:19 2026 GMT
  host: www.flo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: account.flo.com
  https: true
  role: driver / station-owner web login
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:08:02 2026 GMT
  host: store.flo.com
  https: true
  role: Shopify commerce (public MCP + JSON product feeds)
  tls_version: TLSv1.3
- cert_expires: Sep  8 18:01:38 2026 GMT
  host: trust.flo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: Vanta trust center
  tls_version: TLSv1.3
- cert_expires: Oct 21 18:26:22 2026 GMT
  host: network.flo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  role: Salesforce Experience Cloud community portal (OIDC discovery live)
  tls_version: TLSv1.3
- host: auth.flo.com
  https: true
  role: AWS API Gateway (private FLO auth service - 403 Missing Authentication Token on every path)
- host: mqtt-production.ems.flo.com
  https: true
  role: FLO energy-management service (JSON 404 with traceId on every path)
kind: domain-security
layout: security
method: probed
name: Flo Ev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLO, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FLO
provider_slug: flo-ev
slug: flo-ev-domain-security
source_filename: flo-ev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every flo.com host discovered this round\nhosts:\n- host: www.flo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:55:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: account.flo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  role: driver / station-owner web login\n- host: store.flo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:08:02 2026 GMT\n  role: Shopify commerce (public MCP + JSON product feeds)\n- host: trust.flo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: Vanta trust center\n- host: network.flo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:26:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  role: Salesforce Experience\
  \ Cloud community portal (OIDC discovery live)\n- host: auth.flo.com\n  https: true\n  role: AWS API Gateway (private FLO auth service - 403 Missing Authentication Token on every path)\n- host: mqtt-production.ems.flo.com\n  https: true\n  role: FLO energy-management service (JSON 404 with traceId on every path)\ndomains:\n- domain: flo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nsubdomain_census:\n  method: Certificate Transparency (api.certspotter.com, include_subdomains=true)\n  date: '2026-07-27'\n  flo_com_names_observed: 40\n  operational_hosts:\n  - {host: auth.flo.com, resolves: true, http: 403}\n  - {host: authorize.flo.com, resolves: true, http: 200, title: EV Driver Consumer Portal}\n  - {host: station.flo.com, resolves: true, http: 200, title: FLO}\n  - {host: configuration.flo.com, resolves: true, http: 404}\n  - {host: connectionservice.flo.com, resolves: true, http: 000}\n  - {host: csnms.flo.com, resolves: true, http: 404, note:\
  \ Charging Station Network Management System - nginx, no public route}\n  - {host: cc.flo.com, resolves: true, http: 200, title: FLO - Web payment}\n  - {host: edge.flo.com, resolves: true, http: 400}\n  - {host: mqtt-production.ems.flo.com, resolves: true, http: 404}\n  - {host: helpdesk.flo.com, resolves: true, http: 302, note: Freshdesk support portal}\n  - {host: onboarding.flo.com, resolves: true, http: 301}\n  - {host: panel.flo.com, resolves: true, http: 302}\n  - {host: tools.flo.com, resolves: true, http: 403}\n  - {host: 'store.{us,en,fr}.flo.com', resolves: true, note: Shopify regional storefronts}\n  non_resolving_developer_names:\n  - api.flo.com\n  - developer.flo.com\n  - developers.flo.com\n  - docs.flo.com\n  - data.flo.com\n  - emobility.flo.com\n  - ocpi.flo.com\n  - emsp.flo.com\n  - cpo.flo.com\n  - status.flo.com\n  - security.flo.com\n  - partner.flo.com\n  - partners.flo.com\n  - portal.flo.com\n  note: >-\n    FLO runs substantial API infrastructure (an AWS API\
  \ Gateway at auth.flo.com,\n    a CSNMS host, an EMS/MQTT host, an edge host) - all of it private. Every\n    developer-facing name a third party would try does not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flo-ev/refs/heads/main/security/flo-ev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- EV Charging
- Electricity
- Grid
- Demand Response
- Interoperability
- OCPP
- OCPI
- OpenADR
- Charge Point Operator
- Quebec
---
