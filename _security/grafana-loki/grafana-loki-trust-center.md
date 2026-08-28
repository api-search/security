---
certifications:
- SOC 2 Type 2
- ISO 27001
- PCI DSS
- FedRAMP High
- GDPR
- CSA STAR
- EU-US / Swiss-US Data Privacy Framework
description: Grafana Labs publishes a SafeBase-powered Trust Center holding its security reports, certifications and attestations. It covers Grafana Labs as an operator — Grafana Cloud, and therefore Grafana Cloud Logs (hosted Loki). Self-hosted Grafana Loki inherits none of these certifications; they attach to the operator, not to the AGPL software.
kind: trust-center
layout: security
name: Grafana Loki Trust Center
name_suffix: Trust Center
overview: Grafana Loki maintains a public trust center documenting SOC 2 Type 2, ISO 27001, PCI DSS, FedRAMP High, GDPR, CSA STAR, and EU-US / Swiss-US Data Privacy Framework compliance.
provider_name: Grafana Loki
provider_slug: grafana-loki
slug: grafana-loki-trust-center
source_filename: grafana-loki-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nprobe: true\nsource: https://trust.grafana.com/\nurl: https://trust.grafana.com/\ncertifications:\n- SOC 2 Type 2\n- ISO 27001\n- PCI DSS\n- FedRAMP High\n- GDPR\n- CSA STAR\n- EU-US / Swiss-US Data Privacy Framework\nevidence:\n- source: https://trust.grafana.com/\n  keywords:\n  - soc 2\n  - iso/iec 27001\n  - pci dss\n  - pci-dss\n  - fedramp\n  - trust center\n  - gdpr\n  - csa star\nname: Grafana Labs Trust Center\ndescription: Grafana Labs publishes a SafeBase-powered Trust Center holding its security reports, certifications\n  and attestations. It covers Grafana Labs as an operator — Grafana Cloud, and therefore Grafana Cloud\n  Logs (hosted Loki). Self-hosted Grafana Loki inherits none of these certifications; they attach to the\n  operator, not to the AGPL software.\ncertification_count: 7\nscope: Grafana Labs corporate, Grafana Cloud, and Grafana Federal Cloud (FedRAMP High / DoD IL5).\nprobe_note: trust.grafana.com returns\
  \ HTTP 403 with a Cloudflare interstitial to an ordinary crawler;\n  the page demonstrably exists and is linked from https://grafana.com/legal/security-compliance/, which\n  served HTTP 200 and names the same certifications.\ncorroborating_page: https://grafana.com/legal/security-compliance/\nfedramp:\n  level: FedRAMP High\n  offering: Grafana Federal Cloud\n  dod_il: IL5\n  url: https://grafana.com/products/fedramp-federal-cloud/\n  announced: '2025-04-16'\nchecked: '2026-08-27'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafana-loki/refs/heads/main/security/grafana-loki-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001, PCI DSS, FedRAMP High, GDPR, CSA STAR, EU-US / Swiss-US Data Privacy Framework
tags:
- Company
- Logs
- Logging
- Log Aggregation
- Observability
- Monitoring
- Open Source
- LogQL
- OpenTelemetry
- Telemetry
- Kubernetes
- Cloud Native
trust_url: https://trust.grafana.com/
---
