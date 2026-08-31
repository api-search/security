---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 23andme.org
  spf: true
- caa: []
  dmarc: true
  dmarc_aggregate_reporting: true
  dmarc_forensic_reporting: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_subdomain_policy: quarantine
  dnssec: false
  domain: 23andme.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Oct  6 21:49:47 2026 GMT
  host: www.23andme.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: www.23andme.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 301
  https: true
  redirects_to: https://www.23andme.org/
  tls_version: TLSv1.3
- cert_verify: 0 (ok)
  host: api.23andme.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  http_status: 403
  https: true
  tls_version: TLSv1.3
  waf: 'Cloudflare managed challenge (cf-mitigated: challenge)'
kind: domain-security
layout: security
method: probed
name: 23Andme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 23andMe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 23andMe
provider_slug: 23andme
slug: 23andme-domain-security
source_filename: 23andme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  probe-domain-security.py covers the hosts named in apis.yml, which is now the\n  canonical www.23andme.org. The 23andme.com apex and the api.23andme.com host were\n  probed by hand on the same date and appended here, because 23andMe still runs its\n  account, auth, API and support subdomains on 23andme.com even though the consumer\n  site migrated to 23andme.org.\nhosts:\n- host: www.23andme.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:49:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.23andme.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 301\n  redirects_to: https://www.23andme.org/\n- host: api.23andme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_verify: 0 (ok)\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains:\
  \ true\n  hsts_preload: true\n  http_status: 403\n  waf: 'Cloudflare managed challenge (cf-mitigated: challenge)'\ndomains:\n- domain: 23andme.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 23andme.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: quarantine\n  dmarc_pct: 100\n  dmarc_aggregate_reporting: true\n  dmarc_forensic_reporting: true\nfindings:\n- id: no-dnssec\n  detail: Neither 23andme.org nor 23andme.com is DNSSEC-signed (no DS record).\n- id: no-caa\n  detail: >-\n    Neither domain publishes a CAA record, so any public CA may issue for them. Notable\n    for a company holding consumer genetic data.\n- id: dmarc-not-reject\n  detail: >-\n    Both domains sit at p=quarantine rather than p=reject, on both the domain and its\n    subdomains. Aggregate and forensic reporting are configured (dmarcian).\n- id: hsts-strong\n  detail: >-\n    All\
  \ three hosts send HSTS with max-age=63072000 (two years), includeSubDomains and\n    preload.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/23andme/refs/heads/main/security/23andme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Genetics
- Genomics
- DNA Testing
- Ancestry
- Consumer Health
- Bioinformatics
- Precision Medicine
- Pharmacogenomics
- Telehealth
- Health Research
---
