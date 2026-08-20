---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pearpop.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pearpop.ai
  spf: true
hosts:
- cert_expires: Sep 24 07:27:39 2026 GMT
  host: www.pearpop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 20:51:33 2026 GMT
  host: pearpop.ai
  hsts: false
  https: true
  note: Pearpop.AI application host; no Strict-Transport-Security header observed on the sign-in response.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pearpop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PearPop, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PearPop
provider_slug: pearpop
slug: pearpop-domain-security
source_filename: pearpop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pearpop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 07:27:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pearpop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 20:51:33 2026 GMT\n  hsts: false\n  note: Pearpop.AI application host; no Strict-Transport-Security header observed on\n    the sign-in response.\ndomains:\n- domain: pearpop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pearpop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\ndangling_dns:\n- host: api.pearpop.com\n  record: CNAME\n  target: d-xpcnp063c5.execute-api.us-west-2.amazonaws.com\n  resolves: false\n  note: CNAME published but the AWS API Gateway custom-domain target has no A record\n    — the API host is a dangling delegation, not a live API.\n\
  - host: app.pearpop.com\n  record: CNAME\n  target: dhqx0s6nuv8kr.cloudfront.net\n  resolves: false\n- host: brands.pearpop.com\n  record: CNAME\n  target: des2om9aja3af.cloudfront.net\n  resolves: false\nx-evidence:\n  probed: '2026-08-04'\n  resolver: 8.8.8.8\n  method: dig + openssl s_client + HTTP HEAD\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearpop/refs/heads/main/security/pearpop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Influencer Marketing
- Social-Media
- Marketing
- Marketplace
- Talent Management
- Artificial Intelligence
---
