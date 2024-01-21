---
sidebar_position: 1
---

# App Component

Basic Container that Holds Sample Modals and serves as the Main Container for the Web Page:

## App.js Code

```jsx title="App.js"
<div className="App">
  <header className="App-header">
    <img src="https://www.knowbe4.com/hubfs/KB4-logo.svg" className="App-logo" alt="logo" />
    <h1>Modals</h1>
    <br />
    <PopupModal 
      header="What is PhishER?"
      content={
        <div className="embedded-video">
          <div>
            <iframe className="youtube-container" alt="KnowBe4 Holiday Safety Tips" src="https://www.youtube.com/embed/BQ0WrHd3-Jw?si=DLq9tn3xpTM-By-p" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
          <div>
            <p>PhishER is the key ingredient of an essential security workstream. It's your lightweight Security Orchestration, Automation and Response (SOAR) platform to orchestrate your threat response and manage the high volume of potentially malicious email messages reported by your users.  And, with automatic prioritization of emails, PhishER helps your InfoSec and Security Operations team cut through the inbox noise and respond to the most dangerous threats more quickly.</p>
            <p>Additionally, with PhishER you are able to automate the workstream of the 90% of reported emails that are not threats. Incident Response (IR) orchestration can easily deliver immediate efficiencies to your security team, but the potential value is much greater than that.</p>
            <p>With the right strategy and planning, your organization can build a fully orchestrated and intelligent SOC that can contend with today’s threats. PhishER enables a critical workstream to help your IR teams work together to mitigate the phishing threat and is suited for any organization that wants to automatically prioritize and manage potentially malicious messages - accurately and fast! PhishER is available as a stand-alone product or as an add-on option for current KnowBe4 customers.</p>
          </div>
          <ButtonLink 
            label="Visit KnowBe4 Website"
            class="visit-website-button"
            link="https://www.knowbe4.com/"
          />
        </div>
      }
      darkMode={true}
    />
    <br />
    <ToolTipModal 
      header="Tooltip Modal"
      content={<div><p>This is a place to show a short blurb, definition, or additional information.</p></div>}
      darkMode={false}
    />
  </header>
</div>
```

## Elements Included
- Logo
- Popup Modal
- Tooltip Modal
