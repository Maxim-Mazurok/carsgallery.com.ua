# carsgallery.com.ua

**[Demo](https://carsgallery-com-ua-app.herokuapp.com/)**

## Meeting notes
- Client has the logo
- Likes full-screen logo on the black background to appear on the first screen (I don't recommend it, will try during the design phase)
- Likes following websites of their competitors: [AutoBoutique](http://autoboutique.cars.ua/) and [Ukr-Prokat](https://ukr-prokat.com/)
- Provides both selling and renting car services. It should be two separate pages/categories
- "CAR'S GALLERY" - name of the business
- Booking - simple model, just ask for a phone number, name and send a notification to owner (by Email?)
- Terms of rent - they have a document with [rental terms](pages/terms/en.md), should make a page with that
- Rental agreement - they wanted to post a full rental agreement, but it's not ready yet. Reserve a link for it (in footer, probably)
- Contacts - there should be a page with all contacts
  - Бугаёвская, 35 (бизнес-центр "Меркурий"), офис 214 - [2gis](https://2gis.ua/odessa/firm/1970853118168475), [Google Maps](https://goo.gl/maps/VSL4i5RYU3E2)
  - 093 078 99 27 (Viber, WhatsApp, Telegram)
  - 063 120 60 60 (Viber?, WhatsApp?, Telegram?)
  - [Viber group](https://invite.viber.com/?g2=AQA5qjIlkxZcq0lM4QKoGEr1%2BS%2FFniUTJ4%2FmvXkwi4uldvW53T0IQz0%2BeLTvJ51M)
  - [Instagram](https://www.instagram.com/rent_carsgallery_od/)
- Cars should have a picture (upload) and youtube videos (embed)
- Labels for cars - they should be able to add following labels to the car postings: "New arrival", "Sale" ("Новинка", "Акция")
- carsgallery.com.ua - that's the domain name that they decided on
- About company - create a page with the [company description](pages/about/en.md) (make a links from "call", "come to office", etc.)
- Internationalization - English, Russian and Ukrainian
- Callback hunter ([binotel/getcall](http://www.binotel.ua/getcall))
- Only USD currency
- No car categories
- Rental price will vary depending on the rent duration: 1-7 days, 8-29 days and 30+ days.

## Notes
- On the buy/rent car page, I do not want to show "color" and "city" parameters.
  - Color should be clearly seen on the pictures. While adding this parameter might be really tricky, requiring to include all colors and their translations.
  - Business currently operates only in Odessa, so there is no point of adding "city" parameter. And it has same drawbacks, as the "color" parameter.

## Pages
- [ ] Home page
  - [x] Markup
  - [ ] Backend integration
- [ ] Buy
  - [x] Markup
  - [ ] Backend integration
- [ ] Buy single car
  - [ ] Markup
  - [ ] Backend integration
- [ ] Rent
  - [x] Markup
  - [ ] Backend integration
- [ ] Rent single car
  - [ ] Markup
  - [ ] Backend integration
- [x] About us
  - [x] Markup
  - [ ] Backend integration (optional)
- [x] Contacts
  - [x] Markup
  - [ ] Backend integration (optional)

## Tasks
- [ ] Create telegram usernames for both phones (to make links on the website) and set links
- [ ] Get the logo source in original quality
- [x] Use "Прокат" on the second homepage slider
- [x] Get Russian texts:
  - [x] [About](pages/about/ru.md)
  - [x] [Terms](pages/terms/ru.md)
- [x] Get English translations for:
  - [x] [About](pages/about/en.md)
  - [x] [Terms](pages/terms/en.md)
- [x] Get Ukrainian translations for:
  - [x] [About](pages/about/uk.md)
  - [x] [Terms](pages/terms/uk.md)
- [x] Upload placeholder image to the website
- [x] Include rtf documents into the repository and link
- [x] Get all contacts for page
- [x] Configure free SSL-certificate 

## Release check-list
- [ ] Translation
  - [ ] Check that everything is translated
  - [ ] Check that there's no unresolved translations
  - [ ] Disable i18n debug mode
- [ ] Check any eslint issues
  - [ ] Make sure that telegram links are set
- [ ] Run pa11y tests
- [ ] Enable slider animation (add `interval={5000}` to `<Slider/>` in `Home.js`)
- [ ] Make sure everything works fine on hosting
  - Server-side rendering with PHP? [read](https://sebastiandedeyne.com/server-side-rendering-javascript-from-php/)
  - Ask hosting support to enable NodeJS?
  - Setup routing, so that CMS works, and React renders correctly?
  - Use hash-routing strategy for React?
  - Use subdomain for CMS?
- [ ] Set favicon using [generator](https://realfavicongenerator.net/) or something react-specific

## Finances
- [ ] Get $500 after the job is done
- [x] Get 1076 UAH from the client - got 1080 UAH
- [x] Buy hosting and domain - bought for 1076 UAH on Apr 14, 2019.
- [x] Get $100 in advance (total agreed fee is $600)
