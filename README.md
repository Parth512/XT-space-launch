# XT-space-launch

## Live Demo

[Space-XT](https://space-xt-app.herokuapp.com/spaceXLaunch) 

## Technical Stack 

1. **Angular 11** Framework
2. **HTML/CSS** for design (**Media Query** for Responsiveness)
3. **Server Side rendering** implementation
4. Deployement on **Heroku** `https://space-xt-app.herokuapp.com/spaceXLaunch`

## Pre Requisites to run the application locally
1. Clone https://github.com/Parth512/XT-space-launch
2. Checkout branch `master`
3. Run `npm install` for all dependencies
4. To run the project `npm run dev:ssr`

*Angular application will start on `http://localhost:4200/` which will navigate you to `http://localhost:4200/spaceXLaunch`. The app will automatically reload if you change any of the source files.*

---
## Routing Approach in Application

1. By default, page will be loaded on **/spaceXLaunch** ,loading all products without any filter
2. Once any filter is applied, page url will be appended with query parameters to indicate the filter.
   
   *For eg., /spaceXLaunch?launchYear=2008&launchSuccess=All&landingSuccess=All
             /spaceXLaunch?launchYear=2008&launchSuccess=true&landingSuccess=All
             /spaceXLaunch?launchYear=2008&launchSuccess=true&landingSuccess=true*
             
3. Query parameters will be appended in the url until **any** filter is applied.
4. As and when all filters are cleared, query parameters are removed and gets redirected back to **/spaceXLaunch** 
---

## Server Side Rendering 

1. To facilitate web crawlers through search engine optimization(SEO)
2. To improve performance on mobile and low-powered devices
3. Show the first page quickly with a first-contentful paint

## Responsiveness in Application

1. Page has single column layout until 700 px. (Mobile device)
   ![mobile-view](/xt-coding/src/assets/Mobile_view.png)
2. Page has two column layout between 700px and 1024 px. (Tablet device)
   ![tablet-view](/xt-coding/src/assets/Tablet_view..png)
3. Page has three column layout from 1024 px and beyond 1440px. (Desktop device)
   ![desktop-view](/xt-coding/src/assets/Desktop_view.png)
   
---

## Lighthouse Screenshots

SEO & Accessibility
![SEO-Accessibility-image](/xt-coding/src/assets/LightHouse_Accessibility_SEO.png)


