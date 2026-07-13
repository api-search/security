---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: suse.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: documentation.suse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SUSE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SUSE
provider_slug: suse
slug: suse-domain-security
source_filename: suse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: documentation.suse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: suse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suse/refs/heads/main/security/suse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Linux
- Kubernetes
- Enterprise Linux
- Systems Management
- Open Source
- Container Management
---
