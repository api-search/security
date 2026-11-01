---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allakos.com
  spf: true
hosts:
- host: www.allakos.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allakos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allakos, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allakos
provider_slug: allakos
slug: allakos-domain-security
source_filename: allakos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allakos.com\n  https: false\ndomains:\n- domain: allakos.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/allakos/security/allakos-domain-security.yml
summary_line: DMARC
tags:
- Company
---
