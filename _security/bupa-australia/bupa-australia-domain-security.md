---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bupa.com.au
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.bupa.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: portal.api.bupa.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: Azure API Management managed developer portal
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.bupa.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  http_status: 502
  https: true
  role: Azure APIM custom gateway host, behind Imperva; 502 to all anonymous callers
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: partner.bupa.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: Dynamics 365 Power Pages partner portal
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: partnerlogin.bupa.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: Azure AD B2C identity host
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: my.bupa.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: myBupa member portal
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bupa Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bupa Australia, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bupa Australia
provider_slug: bupa-australia
slug: bupa-australia-domain-security
source_filename: bupa-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + developer-portal + identity hosts\nhosts:\n- host: www.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: portal.api.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  role: Azure API Management managed developer portal\n- host: api.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  http_status: 502\n  role: Azure APIM custom gateway host, behind Imperva; 502 to all anonymous callers\n- host: partner.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  role: Dynamics 365 Power Pages partner portal\n- host: partnerlogin.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  role: Azure AD B2C identity host\n- host: my.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  role: myBupa member portal\ndomains:\n- domain: bupa.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes: |\n  Every Bupa Australia host probed negotiates TLS 1.3 and sets HSTS with a\n  one-year max-age; the two consumer-facing hosts (www and partner) additionally\n  set includeSubDomains with preload. The registrable domain publishes\
  \ SPF and a\n  DMARC record at p=reject, the strongest of the three DMARC policies. The gaps\n  are DNSSEC (unsigned) and CAA (no records, so any CA may issue for\n  bupa.com.au). Absence of a record is recorded data, not an inference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bupa-australia/refs/heads/main/security/bupa-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Health Insurance
- Private Health Insurance
- Carrier
- Healthcare
- Claims
- Policy Administration
- Employee Benefits
- Partner Gated
---
