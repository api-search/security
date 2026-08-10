---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ccagriculture.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: mailto:s-user@ccagriculture.com
  dnssec: true
  domain: rawgarden.farm
  spf: true
  spf_record: v=spf1 a mx include:_spf.google.com include:_spf.zendesk.com include:_spf.mlsend.com ~all
hosts:
- cert_expires: Sep 13 21:48:17 2026 GMT
  host: www.ccagriculture.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 16:00:59 2026 GMT
  host: rawgarden.farm
  hsts: false
  https: true
  note: Consumer brand host (Raw Garden). Origin is fronted by Cloudflare and answered HTTP 403 (bot challenge) to the probe, so response headers could not be observed beyond the TLS handshake.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Central Coast Agriculture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Central Coast Agriculture, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Central Coast Agriculture
provider_slug: central-coast-agriculture
slug: central-coast-agriculture-domain-security
source_filename: central-coast-agriculture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ccagriculture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:48:17 2026 GMT\n  hsts: false\n- host: rawgarden.farm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 16:00:59 2026 GMT\n  hsts: false\n  note: >-\n    Consumer brand host (Raw Garden). Origin is fronted by Cloudflare and answered\n    HTTP 403 (bot challenge) to the probe, so response headers could not be observed\n    beyond the TLS handshake.\ndomains:\n- domain: ccagriculture.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rawgarden.farm\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 a mx include:_spf.google.com include:_spf.zendesk.com include:_spf.mlsend.com ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: mailto:s-user@ccagriculture.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/central-coast-agriculture/refs/heads/main/security/central-coast-agriculture-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Agriculture
- Cannabis
- Farming
- Consumer Packaged Goods
- Manufacturing
- California
---
