# Developers Access Paths

[Back to sitemap index](../sitemap-graph.md) | [Open local entry page](http://localhost:4321/en/developers/)

4 canonical pages. Diagram edges show each page's shortest verified path from `/en/`. Diagram nodes and page titles link to the localhost site.

```mermaid
flowchart LR
  n_477322a4d2["Agora Real-time infrastructure for every li...<br/>/en/"]
  n_e58215a330["Customers Built with Agora<br/>/en/customers/"]
  n_87b5c0473f["Developers Build real-time and AI experienc...<br/>/en/developers/"]
  n_f687c83b27["AI Builder Tools Agora<br/>/en/developers/ai-builder-tools/"]
  n_6d50db0ce6["Partner Integrations | Bring AI models to A...<br/>/en/developers/integrate-with-ten/"]
  n_ef8af86654["Agora Partner Gallery<br/>/en/developers/partner-gallery/"]
  n_ba0ff4e4ae["Sitemap<br/>/en/sitemap/"]
  n_477322a4d2 -->|"Footer"| n_e58215a330
  n_e58215a330 -->|"CTA"| n_87b5c0473f
  n_477322a4d2 -->|"Footer"| n_ba0ff4e4ae
  n_ba0ff4e4ae -->|"HTML sitemap"| n_f687c83b27
  n_477322a4d2 -->|"Header"| n_6d50db0ce6
  n_477322a4d2 -->|"Footer"| n_ef8af86654
  click n_87b5c0473f "http://localhost:4321/en/developers/" "_blank"
  click n_f687c83b27 "http://localhost:4321/en/developers/ai-builder-tools/" "_blank"
  click n_6d50db0ce6 "http://localhost:4321/en/developers/integrate-with-ten/" "_blank"
  click n_ef8af86654 "http://localhost:4321/en/developers/partner-gallery/" "_blank"
  click n_477322a4d2 "http://localhost:4321/en/" "_blank"
  click n_e58215a330 "http://localhost:4321/en/customers/" "_blank"
  click n_ba0ff4e4ae "http://localhost:4321/en/sitemap/" "_blank"
  classDef entry fill:#eaf2ff,stroke:#3b6fc4,color:#183867;
  classDef orphan fill:#fff5d6,stroke:#b77900,color:#5c3d00;
  classDef dead fill:#ffe8e6,stroke:#c53b32,color:#671d18;
  class n_477322a4d2 entry;
```

| Page | Primary access path from `/en/` | Other direct canonical entries | Status |
| --- | --- | --- | --- |
| [Developers Build real-time and AI experiences with Agora](http://localhost:4321/en/developers/)<br>`/en/developers/` | [`/en/`](http://localhost:4321/en/) &rarr; **Footer: "Customers"** &rarr; [`/en/customers/`](http://localhost:4321/en/customers/) &rarr; **CTA: "Start building"** &rarr; [`/en/developers/`](http://localhost:4321/en/developers/) | CTA from [`/en/customers/abby/`](http://localhost:4321/en/customers/abby/)<br>CTA from [`/en/customers/airmeet/`](http://localhost:4321/en/customers/airmeet/)<br>CTA from [`/en/customers/artium-academy/`](http://localhost:4321/en/customers/artium-academy/)<br>CTA from [`/en/customers/arutility/`](http://localhost:4321/en/customers/arutility/)<br>+58 more direct sources | Crawlable |
| [AI Builder Tools Agora](http://localhost:4321/en/developers/ai-builder-tools/)<br>`/en/developers/ai-builder-tools/` | [`/en/`](http://localhost:4321/en/) &rarr; **Footer: "Sitemap"** &rarr; [`/en/sitemap/`](http://localhost:4321/en/sitemap/) &rarr; **HTML sitemap: "AI Builder Tools"** &rarr; [`/en/developers/ai-builder-tools/`](http://localhost:4321/en/developers/ai-builder-tools/) | Card from [`/en/developers/`](http://localhost:4321/en/developers/) | Crawlable |
| [Partner Integrations \| Bring AI models to Agora Conversational AI](http://localhost:4321/en/developers/integrate-with-ten/)<br>`/en/developers/integrate-with-ten/` | [`/en/`](http://localhost:4321/en/) &rarr; **Header: "Partner Integrations Bring your AI ..."** &rarr; [`/en/developers/integrate-with-ten/`](http://localhost:4321/en/developers/integrate-with-ten/) | Sitewide header<br>Sitewide mobile navigation<br>CTA from [`/en/conversational-ai/`](http://localhost:4321/en/conversational-ai/)<br>HTML sitemap from [`/en/sitemap/`](http://localhost:4321/en/sitemap/) | Crawlable |
| [Agora Partner Gallery](http://localhost:4321/en/developers/partner-gallery/)<br>`/en/developers/partner-gallery/` | [`/en/`](http://localhost:4321/en/) &rarr; **Footer: "Partners"** &rarr; [`/en/developers/partner-gallery/`](http://localhost:4321/en/developers/partner-gallery/) | Sitewide footer<br>Other from [`/en/about-us/`](http://localhost:4321/en/about-us/)<br>Breadcrumb from [`/en/partner-category/development/`](http://localhost:4321/en/partner-category/development/)<br>Breadcrumb from [`/en/partner-category/enterprise-integration/`](http://localhost:4321/en/partner-category/enterprise-integration/)<br>Breadcrumb from [`/en/partner-category/platform/`](http://localhost:4321/en/partner-category/platform/)<br>+132 more direct sources | Crawlable |
