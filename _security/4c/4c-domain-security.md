---
description: ''
domains:
- caa:
  - trust-provider.com
  - usertrust.com
  - amazon.com
  - amazonaws.com
  - amazontrust.com
  - awstrust.com
  - comodoca.com
  - digicert.com
  - godaddy.com
  - letsencrypt.org
  - sectigo.com
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: 4cinsights.com
  mx: true
  mx_provider: pphosted.com (Proofpoint)
  nameservers: awsdns (Route 53)
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.protection.outlook.com include:aspmx.pardot.com include:sparkpostmail.com ~all
hosts:
- host: 4cinsights.com
  hsts: false
  hsts_max_age: null
  http: true
  http_redirect_to: http://flashtalking.com/social
  http_status: 301
  https: false
  https_note: TLS connect to 443 times out; no HTTPS listener
  server: awselb/2.0
  tls_version: null
- host: www.4cinsights.com
  hsts: false
  hsts_max_age: null
  http: true
  http_redirect_to: http://flashtalking.com/social
  http_status: 301
  https: false
  https_note: TLS connect to 443 times out; no HTTPS listener
  tls_version: null
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 4C Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4C, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 4C
provider_slug: 4c
slug: 4c-domain-security
source_filename: 4c-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  dig + curl/openssl against 4cinsights.com, 4C Insights' own registrable domain, on\n  2026-09-05. probe-domain-security.py returned \"no-hosts\" because apis.yml carries no\n  Website/baseURL for a defunct company, so this file was probed by hand against the\n  domain the company itself used.\nnote: >-\n  The domain survives the company. It resolves (AWS Route 53 nameservers, two A records)\n  and terminates on an AWS elastic load balancer that answers only on port 80 and 301s\n  every path to http://flashtalking.com/social. There is NO HTTPS listener at all — a TLS\n  connect to 443 times out on both the apex and www — which is unusual and is itself the\n  finding: the surviving redirect was never given a certificate. Mail is still live and\n  routed through Proofpoint, with SPF published (Google + Outlook + Pardot + SparkPost)\n  and no DMARC record. Infrastructure and mail routing both belong to the acquirer, not\n \
  \ to 4C.\nhosts:\n- host: 4cinsights.com\n  https: false\n  https_note: TLS connect to 443 times out; no HTTPS listener\n  http: true\n  http_status: 301\n  http_redirect_to: http://flashtalking.com/social\n  server: awselb/2.0\n  tls_version: null\n  hsts: false\n  hsts_max_age: null\n- host: www.4cinsights.com\n  https: false\n  https_note: TLS connect to 443 times out; no HTTPS listener\n  http: true\n  http_status: 301\n  http_redirect_to: http://flashtalking.com/social\n  tls_version: null\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: 4cinsights.com\n  dnssec: false\n  caa:\n  - trust-provider.com\n  - usertrust.com\n  - amazon.com\n  - amazonaws.com\n  - amazontrust.com\n  - awstrust.com\n  - comodoca.com\n  - digicert.com\n  - godaddy.com\n  - letsencrypt.org\n  - sectigo.com\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:spf.protection.outlook.com include:aspmx.pardot.com include:sparkpostmail.com ~all'\n  dmarc: false\n  dmarc_policy: null\n  mx:\
  \ true\n  mx_provider: pphosted.com (Proofpoint)\n  nameservers: awsdns (Route 53)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4c/refs/heads/main/security/4c-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Defunct
- Acquired
- Advertising
- Marketing
- Analytics
- Social Media
- Television
- Audience Intelligence
- Ad Tech
---
