---
description: ''
domains:
- caa:
  - gitbuyer.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gitbuyer.com
  spf: false
hosts:
- host: gitbuyer.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gitbuyer-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gitbuyer-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: gitbuyer-com
provider_slug: gitbuyer-com
slug: gitbuyer-com-domain-security
source_filename: gitbuyer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitbuyer.com\n  https: false\ndomains:\n- domain: gitbuyer.com\n  dnssec: true\n  caa:\n  - gitbuyer.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gitbuyer-com/security/gitbuyer-com-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
