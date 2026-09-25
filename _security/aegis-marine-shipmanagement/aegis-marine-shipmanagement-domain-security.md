---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aegisships.com
  spf: true
hosts:
- cert_expires: Oct 17 23:40:51 2026 GMT
  host: aegisships.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aegis Marine Shipmanagement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aegis Marine Shipmanagement, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aegis Marine Shipmanagement
provider_slug: aegis-marine-shipmanagement
slug: aegis-marine-shipmanagement-domain-security
source_filename: aegis-marine-shipmanagement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aegisships.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:40:51 2026 GMT\n  hsts: false\ndomains:\n- domain: aegisships.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/security/aegis-marine-shipmanagement-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Shipping
- Ship Management
- Maritime
- Marine Transportation
- Oil and Gas
- Crude Oil Tankers
- LNG
- Offshore
- Chartering
- Crew Management
- Logistics
- Guyana
---
