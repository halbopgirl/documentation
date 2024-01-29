---
sidebar_position: 1
---

# App Component

Basic Container that Holds Sample Modals and serves as the Main Container for the Web Page:

## App.js Code

```jsx title="App.js"
<div className="App">
  <header className="App-header">
    <img src="https://yt3.googleusercontent.com/b17saFE1eovJvsLl0BuzYb-rgsyfrdQsSJeDZuTQO2FNoQOGlHYyPb6fIH_5NmStUQm49wy4yw=w1060-fcrop64=1,00005a57ffffa5a8-k-c0xffffffff-no-nd-rj" className="App-logo" alt="logo" />
    <h1>Modals</h1>
    <br />
    <PopupModal 
      header="Who is Kitty Pow?"
      content={
        <div className="embedded-video">
          <div>
            <iframe className="youtube-container" alt="Kitty Pow Music Video" src="https://youtu.be/HnQxJkfVQrk?si=v0kQLHO8FxmfNgkk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
          <div>
            <p>33-year-old pop-punk princess Kitty Pow! hails from Binghamton, NY.  After years on the outskirts of the music industry, she is finally coming out with her breakthrough album in 2024.</p>
          </div>
          <ButtonLink 
            label="Visit Kitty Pow Website"
            class="visit-website-button"
            link="https://www.kittypowmusic.com/"
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
