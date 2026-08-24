---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: insidesales.com
  spf: true
hosts:
- cert_expires: Sep 30 16:20:29 2026 GMT
  host: www.insidesales.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 04:17:12 2026 GMT
  host: helpcenter.insidesales.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: callrecordings.insidesales.com
  https: false
kind: domain-security
layout: security
method: probed
name: Insidesales Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InsideSales (XANT / InsideSales.com), probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: InsideSales (XANT / InsideSales.com)
provider_slug: insidesales-com
slug: insidesales-com-domain-security
source_filename: insidesales-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insidesales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:20:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: helpcenter.insidesales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: callrecordings.insidesales.com\n  https: false\ndomains:\n- domain: insidesales.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nunresolvable_hosts:\n- {host: api.insidesales.com, dns: NXDOMAIN, record: 'CNAME tyk-gateway-103411294.us-east-1.elb.amazonaws.com', note: 'Dangling CNAME into a deleted AWS elastic load balancer — the record survives, the target does not. This is a subdomain-takeover vector as well as a dead API host.'}\n- {host: callrecordings.insidesales.com, dns: SERVFAIL, note: 'The host every Playbooks call-recording URL is built\
  \ on, per the live help article.'}\n- {host: ci-global-api.pdlmpapis.insidesales.com, dns: SERVFAIL, note: 'The API reference host linked from the live Call Recording API article. Parent zone pdlmpapis.insidesales.com also SERVFAILs.'}\n- {host: playbooksmanager.insidesales.com, dns: NODATA, record: 'CNAME d3d22imzfrt4mj.cloudfront.net', note: 'Playbooks Manager App, where an administrator mints the API access key. CloudFront distribution returns no address record.'}\nprobe_note: >-\n  Confirmed against 1.1.1.1 and 8.8.8.8 on 2026-08-23. insidesales.com is served from Route 53\n  (ns-477.awsdns-59.com et al); the marketing, help-center and resources hosts are WP Engine\n  (wp.wpenginepowered.com) and the status host is Atlassian Statuspage.\ndmarc_note: >-\n  No _dmarc.insidesales.com TXT record exists, and no CAA record and no DNSSEC DS record are\n  published for the registrable domain, while the domain does carry live Google Workspace MX. SPF\n  is present.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insidesales-com/refs/heads/main/security/insidesales-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sales
- Sales Engagement
- Sales Automation
- CRM
- Call Recording
- Artificial Intelligence
- Salesforce
- Microsoft Dynamics
- Enterprise Software
---
