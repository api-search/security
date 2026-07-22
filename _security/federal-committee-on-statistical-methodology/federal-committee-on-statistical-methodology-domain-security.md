---
description: ''
domains:
- caa:
  - 0 iodef "mailto:DL.OMB.MAXExtCerts@omb.eop.gov"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686273"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686272"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: statspolicy.gov
  spf: true
hosts:
- cert_expires: Sep 25 21:43:09 2026 GMT
  host: statspolicy.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Committee On Statistical Methodology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Committee on Statistical Methodology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Committee on Statistical Methodology
provider_slug: federal-committee-on-statistical-methodology
slug: federal-committee-on-statistical-methodology-domain-security
source_filename: federal-committee-on-statistical-methodology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statspolicy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: statspolicy.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:DL.OMB.MAXExtCerts@omb.eop.gov\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686273\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686272\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-committee-on-statistical-methodology/refs/heads/main/security/federal-committee-on-statistical-methodology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Statistical Methodology
- Statistics
---
