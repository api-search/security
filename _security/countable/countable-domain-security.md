---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myactionable.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: countable.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:servers.mcsv.net include:7152315.spf08.hubspotemail.net ~all
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.myactionable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.countable.com
  hsts: false
  https: true
  note: legacy Countable host; HTTP 302 to https://www.myactionable.com/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Countable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Countable, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Countable
provider_slug: countable
slug: countable-domain-security
source_filename: countable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myactionable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.countable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n  note: legacy Countable host; HTTP 302 to https://www.myactionable.com/\ndomains:\n- domain: myactionable.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: countable.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:servers.mcsv.net\n    include:7152315.spf08.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countable/refs/heads/main/security/countable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Civic Technology
- Government
- Advocacy
- Political Engagement
- Nonprofit
- SaaS
---
