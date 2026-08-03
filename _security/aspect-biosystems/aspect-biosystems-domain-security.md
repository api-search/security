---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; pct=100; rua=mailto:dmarc@aspectbiosystems.com
  dnssec: false
  domain: aspectbiosystems.com
  mx: google-workspace
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.trustedemail.co include:mg-spf.greenhouse.io include:spf.protection.outlook.com ~all
hosts:
- host: aspectbiosystems.com
  hsts: null
  hsts_max_age: null
  https: null
  note: HTTP/TLS layer INDETERMINATE from the probe network. aspectbiosystems.com resolves to 35.183.91.107 (AWS ca-central-1) but TCP connections to both :443 and :80 time out from this network — an origin-side ASN/geo filter, not an outage. The site was confirmed live and serving HTTPS via an out-of-network reader proxy on the same day. TLS version, certificate expiry, and HSTS could not be measured and are recorded as unknown rather than false.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Aspect Biosystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspect Biosystems, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aspect Biosystems
provider_slug: aspect-biosystems
slug: aspect-biosystems-domain-security
source_filename: aspect-biosystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aspectbiosystems.com\n  https: null\n  note: >-\n    HTTP/TLS layer INDETERMINATE from the probe network. aspectbiosystems.com resolves\n    to 35.183.91.107 (AWS ca-central-1) but TCP connections to both :443 and :80 time\n    out from this network — an origin-side ASN/geo filter, not an outage. The site was\n    confirmed live and serving HTTPS via an out-of-network reader proxy on the same day.\n    TLS version, certificate expiry, and HSTS could not be measured and are recorded as\n    unknown rather than false.\n  tls_version: null\n  hsts: null\n  hsts_max_age: null\ndomains:\n- domain: aspectbiosystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.trustedemail.co include:mg-spf.greenhouse.io\n    include:spf.protection.outlook.com ~all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1;\
  \ p=reject; pct=100; rua=mailto:dmarc@aspectbiosystems.com\n  mx: google-workspace\nx-evidence:\n  probed: '2026-08-02'\n  dns_layer: valid\n  http_layer: unreachable-from-probe-network\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspect-biosystems/refs/heads/main/security/aspect-biosystems-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Regenerative Medicine
- Bioprinting
- Tissue Engineering
- Cell Therapy
- Healthcare
- Canada
---
