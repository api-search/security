---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kompyte.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: kompyte.pro
  note: The application domain has no DMARC record at _dmarc.kompyte.pro and no CAA record. SPF is published and is strict (-all).
  spf: true
  spf_record: v=spf1 include:spf.mailjet.com -all
hosts:
- cert_expires: Oct 29 11:55:02 2026 GMT
  host: kompyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HubSpot-hosted marketing site (www.kompyte.com CNAMEs to sites.hubspot.net).
  tls_version: TLSv1.3
- cert_expires: Oct 11 11:01:23 2026 GMT
  cert_issuer: Google Trust Services WR3
  host: phi.kompyte.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Customer application. The SPA is served from Google Cloud Storage (server: UploadServer) with no HSTS on the static object responses; the API backend behind the same Google Cloud load balancer (x-powered-by: Express) DOES send strict-transport-security: max-age=31536000; includeSubDomains.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kompyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kompyte, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kompyte
provider_slug: kompyte
slug: kompyte-domain-security
source_filename: kompyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the kompyte.com marketing host and the kompyte.pro application host\nhosts:\n- host: kompyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:55:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: HubSpot-hosted marketing site (www.kompyte.com CNAMEs to sites.hubspot.net).\n- host: phi.kompyte.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WR3\n  cert_expires: Oct 11 11:01:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Customer application. The SPA is served from Google Cloud Storage (server: UploadServer) with\n    no HSTS on the static object responses; the API backend behind the same Google Cloud load\n    balancer (x-powered-by: Express) DOES send\n    strict-transport-security: max-age=31536000; includeSubDomains.\ndomains:\n- domain: kompyte.com\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kompyte.pro\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.mailjet.com -all\n  dmarc: false\n  dmarc_policy: null\n  note: >-\n    The application domain has no DMARC record at _dmarc.kompyte.pro and no CAA record. SPF is\n    published and is strict (-all).\nfindings:\n- No CAA record on either domain — any public CA may issue for kompyte.com or kompyte.pro.\n- No DNSSEC on either domain.\n- >-\n  kompyte.com publishes DMARC at p=none (monitor only, no enforcement); kompyte.pro publishes no\n  DMARC record at all, even though it is the domain the customer application and its login live\n  on.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kompyte/refs/heads/main/security/kompyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Competitive Intelligence
- Sales Enablement
- Market Intelligence
- Battlecards
- Win Loss Analysis
- SaaS
- Marketing
---
