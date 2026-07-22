---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fetchrobotics.com
  spf: true
hosts:
- host: fetchrobotics.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Fetch Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fetch Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fetch Robotics
provider_slug: fetch-robotics
slug: fetch-robotics-domain-security
source_filename: fetch-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetchrobotics.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: fetchrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetch-robotics/refs/heads/main/security/fetch-robotics-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Robotics
- Autonomous Mobile Robots
- Warehouse Automation
- ROS
- Robot Operating System
- Material Handling
- Manufacturing
- Fulfillment
- Open Source
---
