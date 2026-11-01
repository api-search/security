---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "eCert.gov.hk"
  - 0 issue "hongkongpost.gov.hk"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: landsd.gov.hk
  spf: true
hosts:
- cert_expires: Mar  6 07:45:43 2027 GMT
  host: landsd.gov.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lands Department Hong Kong Sar Government Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lands Department, Hong Kong SAR Government, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lands Department, Hong Kong SAR Government
provider_slug: lands-department-hong-kong-sar-government
slug: lands-department-hong-kong-sar-government-domain-security
source_filename: lands-department-hong-kong-sar-government-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landsd.gov.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 07:45:43 2027 GMT\n  hsts: false\ndomains:\n- domain: landsd.gov.hk\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"eCert.gov.hk\"\n  - 0 issue \"hongkongpost.gov.hk\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lands-department-hong-kong-sar-government/security/lands-department-hong-kong-sar-government-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Land
- HongKong
- GIS
- PublicServices
---
