---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: shorelinebio.com
  mx: true
  mx_record: shorelinebio-com.mail.protection.outlook.com
  ns:
  - achiel.ns.cloudflare.com
  - selah.ns.cloudflare.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Oct 24 19:11:17 2026 GMT
  cert_issuer: Let's Encrypt
  edge: squarespace
  host: www.shorelinebio.com
  hsts: false
  hsts_max_age: 0
  http_note: Squarespace "Website Expired" holding page — the account has lapsed, no site is served.
  http_status: 404
  https: true
  other_security_headers:
  - 'x-content-type-options: nosniff'
  tls_version: TLSv1.3
- host: shorelinebio.com
  http_note: apex redirects to https://www.shorelinebio.com/, which returns the expired-account page.
  http_status: 404
  https: true
kind: domain-security
layout: security
method: probed
name: Shoreline Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shoreline Biosciences, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Shoreline Biosciences
provider_slug: shoreline-biosciences
slug: shoreline-biosciences-domain-security
source_filename: shoreline-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the company's own registrable domain, 2026-08-27\nnote: >-\n  Probed shorelinebio.com, the domain Shoreline Biosciences itself operated, rather than the\n  forgeglobal.com host carried as the Website pointer — that is a secondary-market venue listing\n  about the company, not a company-controlled host, so its TLS/DNS posture measures Forge Global.\n  shorelinebio.com is still registered and its DNS is served by Cloudflare, but the site behind it\n  is a Squarespace account in the \"Website Expired\" state: both the apex and www answer HTTP 404\n  with a Squarespace holding page. Mail is still routed (MX to Microsoft 365) and SPF is published\n  with a hard fail, so the domain has not been abandoned outright even though the website is gone.\n  HSTS is present but explicitly disabled (max-age=0). No DNSSEC, no CAA, no DMARC record.\nhosts:\n- host: www.shorelinebio.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_issuer: \"Let's Encrypt\"\n  cert_expires: Oct 24 19:11:17 2026 GMT\n  hsts: false\n  hsts_max_age: 0\n  http_status: 404\n  http_note: Squarespace \"Website Expired\" holding page — the account has lapsed, no site is served.\n  edge: squarespace\n  other_security_headers:\n  - 'x-content-type-options: nosniff'\n- host: shorelinebio.com\n  https: true\n  http_status: 404\n  http_note: apex redirects to https://www.shorelinebio.com/, which returns the expired-account page.\ndomains:\n- domain: shorelinebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: false\n  dmarc_policy: null\n  mx: true\n  mx_record: shorelinebio-com.mail.protection.outlook.com\n  ns:\n  - achiel.ns.cloudflare.com\n  - selah.ns.cloudflare.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoreline-biosciences/refs/heads/main/security/shoreline-biosciences-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Immunotherapy
- Oncology
- Stem Cells
- Pharmaceuticals
---
