---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tnlmediagene.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ad2iction.com
  nameservers: cloudflare
  spf: true
  spf_record: v=spf1 mx include:amazonses.com include:mailgun.org ?all
hosts:
- cert_expires: Sep 24 17:07:58 2026 GMT
  host: www.tnlmediagene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: ads.ad2iction.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 13 11:41:22 2026 GMT
  host: www.ad2iction.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tnlmedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TNL Mediagene, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TNL Mediagene
provider_slug: tnlmedia
slug: tnlmedia-domain-security
source_filename: tnlmedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the TNL Mediagene and Ad2iction hosts named in apis.yml\nnote: >-\n  docs.prebid.org is the humanURL for the Ad2iction bidder reference but is operated\n  by Prebid.org, not by TNL Mediagene, so it is deliberately excluded from these\n  results — probing it would credit or penalise this company for a domain it does\n  not control.\nhosts:\n- host: www.tnlmediagene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:07:58 2026 GMT\n  hsts: false\n- host: ads.ad2iction.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: www.ad2iction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:41:22 2026 GMT\n  hsts: false\ndomains:\n- domain: tnlmediagene.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ad2iction.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record:\
  \ 'v=spf1 mx include:amazonses.com include:mailgun.org ?all'\n  dmarc: true\n  dmarc_policy: none\n  nameservers: cloudflare\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tnlmedia/refs/heads/main/security/tnlmedia-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Media
- Publishing
- Advertising
- AdTech
- Marketing
- Digital Media
- Content
- Analytics
- E-Commerce
- Header Bidding
- Programmatic
- Prebid
---
