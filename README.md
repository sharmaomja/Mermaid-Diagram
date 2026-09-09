# Sitemap Graph

This Markdown file contains smaller Mermaid diagrams so the sitemap can be viewed directly in a Markdown preview. Every canonical route is represented either by name below or inside a counted collection family.

## 1. Audit Overview

```mermaid
flowchart TB
  audit["Sitemap audit<br/>811 reported routes"]
  audit --> canonical["Canonical /en/ routes<br/>298"]
  audit --> legacy["Legacy and root variants<br/>513"]

  canonical --> healthy["Crawlable and reachable<br/>266"]
  canonical --> hidden["Non-crawlable orphans<br/>32"]
  healthy -->|"subset"| deadends["Crawlable dead ends<br/>11"]

  legacy --> broken["Rendered 404 links<br/>424"]
  legacy --> redirects["Configured redirects<br/>974"]
  redirects --> valid["Valid destinations<br/>939 entries"]
  redirects --> missing["Missing destinations<br/>35 entries / 7 pages"]

  classDef good fill:#e8f7ee,stroke:#18864b,color:#103d25;
  classDef warn fill:#fff5d6,stroke:#b77900,color:#5c3d00;
  classDef bad fill:#ffe8e6,stroke:#c53b32,color:#671d18;
  classDef info fill:#eaf2ff,stroke:#3b6fc4,color:#183867;
  class healthy,valid good;
  class hidden,deadends,legacy warn;
  class broken,missing bad;
  class audit,canonical,redirects info;
```

## 2. Canonical Page Families

The 298 canonical routes consist of 194 routes in repeatable collections and 104 other routes detailed in the next section.

```mermaid
flowchart LR
  canonical["Canonical /en/<br/>298 routes"]
  canonical --> collections["Collection families<br/>194 routes"]
  canonical --> other["Other named pages<br/>104 routes"]

  collections --> customers["Customers<br/>58"]
  collections --> partners["Partners<br/>64"]
  collections --> partnerCategories["Partner categories<br/>6"]
  collections --> pricing["Pricing<br/>26"]
  collections --> events["Events<br/>15"]
  collections --> eventCategories["Event categories<br/>4"]
  collections --> extensions["Extensions<br/>14"]
  collections --> developers["Developers<br/>4"]
  collections --> tools["Tools<br/>3"]

  other --> company["Company and platform"]
  other --> legal["Legal, security and trust"]
  other --> forms["Forms and conversion"]
  other --> resources["Campaigns and resources"]

  classDef family fill:#eaf2ff,stroke:#3b6fc4,color:#183867;
  classDef group fill:#f5f5f5,stroke:#666,color:#222;
  class canonical,collections,other family;
  class customers,partners,partnerCategories,pricing,events,eventCategories,extensions,developers,tools,company,legal,forms,resources group;
```

### Collection Family Contents

| Family | Routes represented |
| --- | --- |
| Customers | `/en/customers/` plus 57 customer stories |
| Partners | `/en/partners/` plus 63 partner profiles |
| Partner categories | Development, enterprise integration, platform, reseller, SaaS, technology |
| Pricing | `/en/pricing/` plus 25 pricing detail pages |
| Events | `/en/events/` plus 14 event pages |
| Event categories | On demand, online virtual event, product, upcoming |
| Extensions | `/en/extensions/` plus 13 extension, policy, FAQ, application, and thank-you pages |
| Developers | `/en/developers/`, AI Builder Tools, Integrate with TEN, Partner Gallery |
| Tools | App Builder, Flexible Classroom, UI Kits |

## 3. Other Canonical Pages

### Company And Platform

```mermaid
flowchart LR
  group["Company and platform"]
  group --> home["Home<br/>/en/"]
  group --> company["About Us<br/>Careers + Open Positions<br/>Agora Management<br/>Agora for Startups"]
  group --> support["Customer Support<br/>Support Plans<br/>Explore"]
  group --> platform["Conversational AI<br/>Platform Advantage<br/>Software-Defined Real-Time Network<br/>WebRTC<br/>Unity"]
  group --> comparisons["Amazon IVS comparison<br/>Twilio migration<br/>Twilio / Zoom / Agora comparison"]
```

### Legal, Security And Trust

```mermaid
flowchart LR
  group["Legal, security and trust"]
  group --> privacy["Privacy Policy<br/>Legacy Privacy Policy<br/>Processor Privacy Statement<br/>Cookie Policy<br/>CCPA<br/>Data Privacy Framework"]
  group --> terms["Terms of Service<br/>Acceptable Use Policy<br/>SDK Licence Agreement<br/>Third-Party Licenses<br/>Certificate Program Terms"]
  group --> safety["Security<br/>Compliance<br/>Trust & Safety<br/>Content Standards<br/>Infringement Policy"]
  group --> rte["RTE 2024:<br/>Terms<br/>Content Guidelines<br/>Infringement Policy"]
  group --> utility["HTML Sitemap<br/>Trust & Safety thank-you"]
```

### Forms And Conversion Pages

```mermaid
flowchart LR
  group["Forms and conversion"]
  group --> sales["Schedule a Demo + thank-you<br/>Talk to Us + thank-you<br/>General thank-you"]
  group --> partner["Become a Partner<br/>Development Partner<br/>Embedded Reseller<br/>Reseller Partner<br/>Technology Partner<br/>Partner Gallery"]
  group --> ai["Agent Studio pricing request<br/>ConvoAI Marketplace<br/>Device Kit request<br/>Engine request"]
  group --> iot["IoT SDK information request<br/>IoT SDK pricing request"]
```

### Campaigns And Resources

Each item ending in `+ TY` includes its separate thank-you route.

```mermaid
flowchart TB
  group["Campaigns and resources"]
  group --> webinars["Webinars"]
  group --> guides["Guides and ebooks"]
  group --> commerce["Commerce and social"]
  group --> misc["Other campaigns"]

  webinars --> w1["Advances in AI for Telehealth + TY"]
  webinars --> w2["Advances in AR/VR for Telehealth + TY"]
  webinars --> w3["EdTech scalability + TY"]
  webinars --> w4["Metaverse webinar + TY"]
  webinars --> w5["Social app engagement webinar + TY"]

  guides --> g1["Conversational AI Benchmark"]
  guides --> g2["Customized Online Tutoring + TY"]
  guides --> g3["Professional Training with RTE + TY"]
  guides --> g4["Successful Telehealth + TY"]
  guides --> g5["Innovative Games ebook + TY"]
  guides --> g6["Gaming retention + TY"]
  guides --> g7["Gartner Live Commerce guide"]
  guides --> g8["Gartner Market Guide + TY"]

  commerce --> c1["Boost In-App Engagement + TY"]
  commerce --> c2["Enable In-Game Chat"]
  commerce --> c3["Social Gaming Experiences + TY"]
  commerce --> c4["Social App Monetization + TY"]
  commerce --> c5["Live Commerce Insights + TY"]
  commerce --> c6["Scaling Digital Commerce + TY"]
  commerce --> c7["Retail Revolution + TY"]

  misc --> m1["CEE 2024 Call for Speakers"]
  misc --> m2["Harness Social Interactions + TY"]
  misc --> m3["Future of Work + TY"]
  misc --> m4["Secret Ingredient for Human Interaction + TY"]
  misc --> m5["Metaverse availability webinar"]
  misc --> m6["Unlock the Metaverse + TY"]
  misc --> m7["Chat-Powered Social Games + TY"]
  misc --> m8["Solution Brief thank-you"]
  misc --> m9["Standalone ebook thank-you"]
```

Additional standalone completion routes represented above:

- `/en/how-to-enable-in-game-chat-to-connect-players-and-boost-engagement/thank-you/`
- `/en/real-time-engagement-reshaping-the-future-of-work/thank-you/`

## 4. Pages Requiring Review

```mermaid
flowchart TB
  review["Review queue"]
  review --> dead["11 crawlable dead ends"]
  review --> orphan["3 unusual non-crawlable orphans"]
  review --> redirect["7 missing redirect destinations"]

  dead --> eventDead["Events:<br/>Colombia Tech Week<br/>IBC Convention<br/>IEEE RTC Conference<br/>Mexico Tech Week<br/>Social Commerce Conference"]
  dead --> otherDead["Other:<br/>AR/VR Telehealth webinar<br/>Conversational AI Benchmark<br/>Extensions FAQ<br/>Gaming retention guide<br/>Legacy Privacy Policy<br/>HTML Sitemap"]

  orphan --> o1["/en/convo-ai-microsoft-marketplace/"]
  orphan --> o2["/en/partner-gallery/"]
  orphan --> o3["/en/partners/"]

  redirect --> missingCustomers["Missing customers:<br/>Fuzozo<br/>Gabb<br/>Mysivi<br/>Open English<br/>Picslo<br/>Sine Wave<br/>Soma"]

  classDef warn fill:#fff5d6,stroke:#b77900,color:#5c3d00;
  classDef bad fill:#ffe8e6,stroke:#c53b32,color:#671d18;
  class dead,eventDead,otherDead,orphan,o1,o2,o3 warn;
  class redirect,missingCustomers bad;
```

## 5. Legacy Link Problems

```mermaid
flowchart LR
  legacy["513 legacy/root variants"]
  legacy --> broken["424 rendered 404 links"]
  broken --> customers["Customer templates<br/>342"]
  broken --> explore["Explore cards<br/>68"]
  broken --> other["Extensions/developers<br/>14"]

  customers --> customerIndex["/customers/customers.html<br/>228"]
  customers --> developers["/customers/developers.html<br/>114"]

  legacy --> note["Localhost rendered aliases<br/>instead of executing redirects"]

  classDef warn fill:#fff5d6,stroke:#b77900,color:#5c3d00;
  classDef bad fill:#ffe8e6,stroke:#c53b32,color:#671d18;
  class legacy,note warn;
  class broken,customers,explore,other,customerIndex,developers bad;
```

For full URL-level evidence, use [`sitemap.json`](./sitemap.json). For findings and recommended actions, use [`sitemap-report.md`](./sitemap-report.md).
