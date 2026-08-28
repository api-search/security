---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: selkirkpharma.com
  spf: true
hosts:
- host: www.selkirkpharma.com
  https: false
kind: domain-security
layout: security
method: probed
name: Selkirk Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Selkirk Pharma, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Selkirk Pharma
provider_slug: selkirk-pharma
slug: selkirk-pharma-domain-security
source_filename: selkirk-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  www.selkirkpharma.com and selkirkpharma.com (Webflow, proxy-ssl.webflow.com / AWS Global\n  Accelerator) REFUSED the TLS handshake from every client available to this probe — curl\n  (LibreSSL 3.3.6), python ssl and openssl s_client 3.6.2 all received alert 40\n  (handshake_failure) at both TLSv1.2 and TLSv1.3, with and without ALPN. `https: false` above\n  therefore records what OUR probe observed, NOT a claim that the site does not serve HTTPS: port\n  80 answers 301 to the https:// URL, and the site is reachable in an ordinary browser. Treat the\n  https/tls_version/hsts fields for this host as unmeasured rather than absent. DNS records were\n  measured directly and are reliable: SPF present (Proofpoint Essentials + Microsoft 365 +\n  ConnectWise + HubSpot), DMARC present at p=none (no enforcement, no rua/ruf reporting address),\n  no CAA record, no DNSSEC (DS\
  \ absent), nameservers ns71/ns72.domaincontrol.com (GoDaddy), mail\n  at mx1/mx2-us1.ppe-hosted.com.\nhosts:\n- host: www.selkirkpharma.com\n  https: false\ndomains:\n- domain: selkirkpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/selkirk-pharma/refs/heads/main/security/selkirk-pharma-domain-security.yml
summary_line: DMARC
tags:
- Company
- Pharmaceuticals
- Contract Manufacturing
- CDMO
- Sterile Injectables
- Aseptic Fill Finish
- Biologics
- Life Sciences
- Clinical Trials
- Manufacturing
---
