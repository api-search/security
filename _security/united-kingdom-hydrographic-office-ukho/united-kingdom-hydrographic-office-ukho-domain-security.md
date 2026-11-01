---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ukho.gov.uk
  spf: true
hosts:
- cert_expires: Jan 14 23:17:15 2027 GMT
  host: www.ukho.gov.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: United Kingdom Hydrographic Office Ukho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Kingdom Hydrographic Office (UKHO), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: United Kingdom Hydrographic Office (UKHO)
provider_slug: united-kingdom-hydrographic-office-ukho
slug: united-kingdom-hydrographic-office-ukho-domain-security
source_filename: united-kingdom-hydrographic-office-ukho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukho.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:17:15 2027 GMT\n  hsts: false\ndomains:\n- domain: ukho.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/united-kingdom-hydrographic-office-ukho/security/united-kingdom-hydrographic-office-ukho-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hydrography
- Nautical Charts
- Maritime Navigation
- Defence
- Marine Data
- Admiralty Products
---
