# Hjem drinks

Drinksopskrifter til cocktailkortet i Hjem, mit eget Home Assistant-dashboard. 685 drinks på dansk, alle med billede. 310 af dem kommer fra [TheCocktailDB](https://www.thecocktaildb.com) og er oversat til dansk. Se [Billeder](#billeder) for, hvor billederne kommer fra.

Hjem henter listen herfra og viser den som standardmenu. "Hvad kan jeg lave?" i appen søger i den ud fra det, du har i skabet.

## Kategorier

| Kategori | Drinks |
|---|---|
| Gin | 108 |
| Rom | 100 |
| Vodka | 88 |
| Likør | 77 |
| Alkoholfri | 58 |
| Små Shots | 54 |
| Kaffe & dessert | 54 |
| Whisky | 49 |
| Spritz | 47 |
| Tequila | 28 |
| Cognac & brandy | 22 |

## Format

`drinks.json` er en liste. Hver drink ser sådan ud:

```json
{
  "n": "Negroni",
  "c": "Gin",
  "d": "Bitter, sød og stærk på én gang",
  "i": ["3 cl gin", "3 cl Campari", "3 cl sød vermouth", "Appelsinskive", "Isterninger"],
  "m": "Rør det hele med is i et røreglas og si over i et glas med en stor isterning."
}
```

| Felt | Indhold | Højst |
|---|---|---|
| `n` | Navn | 40 tegn |
| `c` | Kategori | 20 tegn |
| `d` | Kort beskrivelse | 120 tegn |
| `i` | Ingredienser, én pr. linje, med mængde i cl | 14 linjer á 60 tegn |
| `m` | Sådan gør du | 400 tegn |
| `g` | Billede (valgfrit), sti i repoet, fx `billeder/negroni.jpg` | 70 kB |

Skriv ingredienserne med almindelige navne (`gin`, `hvid rom`, `limesaft`, `sukkersirup`), så "Hvad kan jeg lave?" i Hjem kan genkende flaskerne. Pynt som `Appelsinskive` og alt, der starter med `Evt.`, tæller ikke med.

## Tilføj en drink

Ret `drinks.json` og lav en pull request. Tjek, at filen stadig er gyldig JSON.

## Billeder

Billederne ligger i `billeder/`. Læg en ny som JPG (højst ca. 360 px og 70 kB), og skriv stien i `g`.

### Hvor billederne kommer fra

| Kilde | Billeder |
|---|---|
| Folderne (Råstoff, CUBA, Pure Shots, BARMIX, Harlegin, Små Shots) | 109 |
| [TheCocktailDB](https://www.thecocktaildb.com), brugt med tilladelse | 379 |
| [Wikimedia Commons](https://commons.wikimedia.org), fri licens (se listen herunder) | 101 |
| Tegnet til Hjem | 96 |

Billederne fra TheCocktailDB og Wikimedia Commons er beskåret og skaleret ned til 288 x 360 px.

### Fotos fra Wikimedia Commons

Fotograf og licens står herunder. Billederne er ændret (beskåret og skaleret ned). CC BY-SA-billederne må bruges videre under samme licens.

| Drink | Originalt billede | Fotograf | Licens |
|---|---|---|---|
| Adios | [Adios Motherfucker Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Adios_Motherfucker_Cocktail.jpg) | Will Shenton | CC BY-SA 3.0 |
| Adonis | [Adonis.png](https://commons.wikimedia.org/wiki/File:Adonis.png) | Bruce The Deus | CC BY-SA 4.0 |
| Air Mail | [Air Mail Cocktail.png](https://commons.wikimedia.org/wiki/File:Air_Mail_Cocktail.png) | Matthias Friedlein (www.augustine-bar.de) | CC BY-SA 4.0 |
| Aperol Sour | [Aperol Sour in Schmitz Katze in Tübingen an der Bar.jpg](https://commons.wikimedia.org/wiki/File:Aperol_Sour_in_Schmitz_Katze_in_Tübingen_an_der_Bar.jpg) | Dktue | CC0 |
| Aperol Spritz | [Aperol Spritz 2014a.jpg](https://commons.wikimedia.org/wiki/File:Aperol_Spritz_2014a.jpg) | Geolina163 | CC BY-SA 4.0 |
| Arnold Palmer | [My new obsession the arnold palmer!!! (5184944881).jpg](https://commons.wikimedia.org/wiki/File:My_new_obsession_the_arnold_palmer!!!_%285184944881%29.jpg) | irina slutsky from san francisco, USA | CC BY 2.0 |
| Baby Guinness | [Baby Guinness.jpg](https://commons.wikimedia.org/wiki/File:Baby_Guinness.jpg) | Brian Child | CC BY-SA 2.0 |
| Bacardi Cocktail | [Bacardi cocktail.jpg](https://commons.wikimedia.org/wiki/File:Bacardi_cocktail.jpg) | Luigi Manzo | CC BY 3.0 |
| Baileys Kaffe | [Irish coffee at Emerils.jpg](https://commons.wikimedia.org/wiki/File:Irish_coffee_at_Emerils.jpg) | Coastie Wife 2008 | CC BY 2.0 |
| Baileys på is | [Baileys and ice 01.jpg](https://commons.wikimedia.org/wiki/File:Baileys_and_ice_01.jpg) | Alessio Sbarbaro User_talk:Yoggysot | GFDL / CC BY-SA 3.0 |
| Bee's Knees | [Bee's Knees.jpg](https://commons.wikimedia.org/wiki/File:Bee's_Knees.jpg) | Will Shenton | CC BY-SA 3.0 |
| Between the Sheets | [Between The Sheets Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Between_The_Sheets_Cocktail.jpg) | Zach | CC BY-SA 4.0 |
| Black Russian | [Black Russian.jpg](https://commons.wikimedia.org/wiki/File:Black_Russian.jpg) | Will Shenton | CC BY-SA 3.0 |
| Blood and Sand | [VTR - Blood and Sand.jpg](https://commons.wikimedia.org/wiki/File:VTR_-_Blood_and_Sand.jpg) | Edsel Little | CC BY-SA 2.0 |
| Bloody Maria | [Bloody Maria Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Bloody_Maria_Cocktail.jpg) | Catprisbrey | CC BY-SA 4.0 |
| Bloody Mary | [Bloody Mary Coctail with celery stalk - Evan Swigart.jpg](https://commons.wikimedia.org/wiki/File:Bloody_Mary_Coctail_with_celery_stalk_-_Evan_Swigart.jpg) | Evan Swigart from Chicago, USA | CC BY 2.0 |
| Blue Hawaiian | [Bluehawaiian.jpg](https://commons.wikimedia.org/wiki/File:Bluehawaiian.jpg) | Monoukotori at English Wikipedia | Public domain |
| Blue Lagoon uden alkohol | [Blue Lagoon at the Mandarin Oriental, Washington DC.jpg](https://commons.wikimedia.org/wiki/File:Blue_Lagoon_at_the_Mandarin_Oriental,_Washington_DC.jpg) | John Phelan | CC BY-SA 3.0 |
| Boulevardier | [VTR Happy Hour - Boulevardier.jpg](https://commons.wikimedia.org/wiki/File:VTR_Happy_Hour_-_Boulevardier.jpg) | Edsel Little | CC BY-SA 2.0 |
| Brain Hemorrhage | [P1020647 (brain haemorrhage).jpg](https://commons.wikimedia.org/wiki/File:P1020647_%28brain_haemorrhage%29.jpg) | Grant Mitchell (Grant Mitchell) | CC BY 2.0 |
| Brandy Alexander | [Brandy alexander.jpg](https://commons.wikimedia.org/wiki/File:Brandy_alexander.jpg) | Jason Lam | CC BY 2.0 |
| Breakfast Martini | [Breakfast Martini.jpg](https://commons.wikimedia.org/wiki/File:Breakfast_Martini.jpg) | popvoid | CC BY 2.0 |
| Bronx | [Bronx (cocktail).jpg](https://commons.wikimedia.org/wiki/File:Bronx_%28cocktail%29.jpg) | Stuart Webster | CC BY 2.0 |
| Caipiroska | [Caipiroska.JPG](https://commons.wikimedia.org/wiki/File:Caipiroska.JPG) | Guitardemon666 | Public domain |
| Campari Orange | [Garibaldi cocktail.jpg](https://commons.wikimedia.org/wiki/File:Garibaldi_cocktail.jpg) | BanjoZebra | CC BY 4.0 |
| Campari Spritz | [20120704 170702 venezia 1584.jpg](https://commons.wikimedia.org/wiki/File:20120704_170702_venezia_1584.jpg) | Gunther H.G. Geick | CC BY-SA 4.0 |
| Cape Codder | [Cape Codder, Tommy Doyles Irish Pub, Hyannis MA.jpg](https://commons.wikimedia.org/wiki/File:Cape_Codder,_Tommy_Doyles_Irish_Pub,_Hyannis_MA.jpg) | John Phelan | CC BY-SA 3.0 |
| Carajillo | [Café Carajillo2.jpg](https://commons.wikimedia.org/wiki/File:Café_Carajillo2.jpg) | Shht! | CC BY 2.0 |
| Chokolademilkshake | [Chocolate milkshake.jpg](https://commons.wikimedia.org/wiki/File:Chocolate_milkshake.jpg) | Hegde Neha | CC BY-SA 4.0 |
| Corpse Reviver No. 2 | [Corpse Reviver 2.jpg](https://commons.wikimedia.org/wiki/File:Corpse_Reviver_2.jpg) | Will Shenton | CC BY-SA 3.0 |
| El Presidente | [El Presidente Cocktail.jpg](https://commons.wikimedia.org/wiki/File:El_Presidente_Cocktail.jpg) | Cocktailmarler | CC BY-SA 4.0 |
| Espresso Tonic | [Espresso and tonic 20150418 2.jpg](https://commons.wikimedia.org/wiki/File:Espresso_and_tonic_20150418_2.jpg) | Bex Walton | CC BY 2.0 |
| Frozen Margarita | [Café Bar Revolución 3.jpg](https://commons.wikimedia.org/wiki/File:Café_Bar_Revolución_3.jpg) | https://www.flickr.com/photos/tjeerd/ | CC BY 2.0 |
| Fuzzy Navel | [Fuzzy navel 01.jpg](https://commons.wikimedia.org/wiki/File:Fuzzy_navel_01.jpg) | 逃亡者 (ja:利用者:逃亡者) | Public domain |
| Garibaldi | [Garibaldi cocktail bright.jpg](https://commons.wikimedia.org/wiki/File:Garibaldi_cocktail_bright.jpg) | User:BanjoZebra | CC BY 4.0 |
| Gibson | [Gibson cocktail.jpg](https://commons.wikimedia.org/wiki/File:Gibson_cocktail.jpg) | SteveR- | CC BY 2.0 |
| Gin Basil Smash | [Gin Basil Smash.jpg](https://commons.wikimedia.org/wiki/File:Gin_Basil_Smash.jpg) | Erich Wagner (www.eventografie.de) | CC BY-SA 4.0 |
| Gløgg | [Glögg kastrull.JPG](https://commons.wikimedia.org/wiki/File:Glögg_kastrull.JPG) | Mr.choppers | CC BY-SA 3.0 / GFDL |
| Godiva Martini | [Chocolate martinis at the Fairmont Washington DC - Sarah Stierch.jpg](https://commons.wikimedia.org/wiki/File:Chocolate_martinis_at_the_Fairmont_Washington_DC_-_Sarah_Stierch.jpg) | Missvain | CC BY 4.0 |
| Grenadine Sunrise | [Tequila Sunrise 2013.JPG](https://commons.wikimedia.org/wiki/File:Tequila_Sunrise_2013.JPG) | stavros1 | CC BY 3.0 |
| Hanky Panky | [Hanky Panky cocktail.jpg](https://commons.wikimedia.org/wiki/File:Hanky_Panky_cocktail.jpg) | Tim Sackton from Somerville, MA | CC BY-SA 2.0 |
| Hemingway Daiquiri | [Hemingway Daiquiri.jpg](https://commons.wikimedia.org/wiki/File:Hemingway_Daiquiri.jpg) | Achim Schleuning (E-Mail: comander02_de@yahoo.de) | CC BY-SA 3.0 de |
| Hindbær Lemonade | [Raspberry lemonade on a wooden table. Iced summer drink. (43108065435).jpg](https://commons.wikimedia.org/wiki/File:Raspberry_lemonade_on_a_wooden_table._Iced_summer_drink._%2843108065435%29.jpg) | Artem Beliaikin from Moscow, Russia | CC0 |
| Hjemmelavet Lemonade | [Homemade lemonade at restaurant Visums, Riga.jpg](https://commons.wikimedia.org/wiki/File:Homemade_lemonade_at_restaurant_Visums,_Riga.jpg) | JIP | CC BY-SA 4.0 / GFDL |
| Hot Buttered Rum | [Hot buttered rum.jpg](https://commons.wikimedia.org/wiki/File:Hot_buttered_rum.jpg) | urban.houstonian | CC BY 2.0 |
| Hugo | [15-09-26-RalfR-WLC-0059.jpg](https://commons.wikimedia.org/wiki/File:15-09-26-RalfR-WLC-0059.jpg) | © Ralf Roletschek Ralf Roletschek (1963–) | FAL / CC BY-SA 3.0 |
| Hurricane | [Hurricane at Pat O'Brien's.JPG](https://commons.wikimedia.org/wiki/File:Hurricane_at_Pat_O'Brien's.JPG) | NOLAskip | CC BY-SA 3.0 |
| Hvid Sangria | [White Sangria at the Marina de Alvor (36512202173).jpg](https://commons.wikimedia.org/wiki/File:White_Sangria_at_the_Marina_de_Alvor_%2836512202173%29.jpg) | Eduard Marmet | CC BY-SA 2.0 |
| Hvidvinsspritzer | [White wine spritzer.jpg](https://commons.wikimedia.org/wiki/File:White_wine_spritzer.jpg) | André Hofmeister | CC BY-SA 2.0 |
| Ingefær Mule | [Sielu Mocktail - Alma, Lisbon (52740512504).jpg](https://commons.wikimedia.org/wiki/File:Sielu_Mocktail_-_Alma,_Lisbon_%2852740512504%29.jpg) | Haydn Blackey from Cardiff, Wales | CC BY-SA 2.0 |
| Iskaffe | [Iced Ipoh White Coffee.jpg](https://commons.wikimedia.org/wiki/File:Iced_Ipoh_White_Coffee.jpg) | KtMystic | CC BY-SA 4.0 |
| Jack & Cola | [Jack & Coke at Encounter Restaurant & Bar at Los Angeles International Airport (11300470795).jpg](https://commons.wikimedia.org/wiki/File:Jack_&_Coke_at_Encounter_Restaurant_&_Bar_at_Los_Angeles_International_Airport_%2811300470795%29.jpg) | Sam Howzit | CC BY 2.0 |
| Jordbærmilkshake | [Strawberry milk shake (cropped).jpg](https://commons.wikimedia.org/wiki/File:Strawberry_milk_shake_%28cropped%29.jpg) | Renee Comet (Photographer) | Public domain |
| Jungle Bird | [Jungle Bird.jpg](https://commons.wikimedia.org/wiki/File:Jungle_Bird.jpg) | Atlantis Tiki Bar | CC BY-SA 4.0 |
| Jägerbomb | [Jagerbomb.jpg](https://commons.wikimedia.org/wiki/File:Jagerbomb.jpg) | ScottMacGregor1985 at English Wikipedia | Public domain |
| Kamikaze Shot | [Shot Kamikaze.jpg](https://commons.wikimedia.org/wiki/File:Shot_Kamikaze.jpg) | pandrinkowiec | CC BY-SA 4.0 |
| Kokos Mojito | [Coconut lime mojito (29951677011).jpg](https://commons.wikimedia.org/wiki/File:Coconut_lime_mojito_%2829951677011%29.jpg) | Lauren Topor from Phoenix | CC BY 2.0 |
| Mango Lassi Mocktail | [Lassi de mango.JPG](https://commons.wikimedia.org/wiki/File:Lassi_de_mango.JPG) | ProtoplasmaKid | CC BY-SA 4.0 |
| Martinez | [Martinez Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Martinez_Cocktail.jpg) | Will Shenton | CC BY-SA 3.0 |
| Midori Sour | [Midori Sour (3804267959).jpg](https://commons.wikimedia.org/wiki/File:Midori_Sour_%283804267959%29.jpg) | Shoshanah | CC BY 2.0 |
| Mudslide | [Mudslide cocktail with chocolate - tumbler (Italy, 2023).png](https://commons.wikimedia.org/wiki/File:Mudslide_cocktail_with_chocolate_-_tumbler_%28Italy,_2023%29.png) | Bruce The Deus | CC BY-SA 4.0 |
| Naked & Famous | [Naked and Famous cocktail.jpg](https://commons.wikimedia.org/wiki/File:Naked_and_Famous_cocktail.jpg) | Rascalisimo | CC BY 4.0 |
| Navy Grog | [Navy Grog.jpg](https://commons.wikimedia.org/wiki/File:Navy_Grog.jpg) | Taken by Hayford Peirce. Photoshopped by David M. Alexander. | CC BY-SA 3.0 |
| Negroni Sbagliato | [Negroni sbagliato.jpg](https://commons.wikimedia.org/wiki/File:Negroni_sbagliato.jpg) | Wine Dharma | CC BY 2.0 |
| Ouzo og vand | [Ouzo.jpg](https://commons.wikimedia.org/wiki/File:Ouzo.jpg) | de:Benutzer:Udm, | GFDL / CC BY-SA 3.0 |
| Paloma Spritz | [Paloma Spritz - Purezza 2024-12-17.jpg](https://commons.wikimedia.org/wiki/File:Paloma_Spritz_-_Purezza_2024-12-17.jpg) | Andy Li | CC0 |
| Paper Plane | [Taub Family Outpost - June 11 2021 - Sarah Stierch 02.jpg](https://commons.wikimedia.org/wiki/File:Taub_Family_Outpost_-_June_11_2021_-_Sarah_Stierch_02.jpg) | Missvain | CC BY 4.0 |
| Peach Iced Tea | [Peach iced tea with orange slices.jpg](https://commons.wikimedia.org/wiki/File:Peach_iced_tea_with_orange_slices.jpg) | Baoothersks | CC BY-SA 4.0 |
| Pharisäer | [Farisæer.jpg](https://commons.wikimedia.org/wiki/File:Farisæer.jpg) | MaikeBred | CC BY-SA 3.0 |
| Pickleback | [Pickleback.jpg](https://commons.wikimedia.org/wiki/File:Pickleback.jpg) | Derek Clark from Vancouver, Canada | CC BY 2.0 |
| Pimm's Cup | [Pimm s-Cup-Nr-1-Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Pimm_s-Cup-Nr-1-Cocktail.jpg) | Charles Clavadetscher | Public domain |
| Pink Gin Tonic | [Pink Gin Tonic.jpg](https://commons.wikimedia.org/wiki/File:Pink_Gin_Tonic.jpg) | Sezenkerem | CC BY-SA 4.0 |
| Queen's Park Swizzle | [Trader vic's queens park swizzle.jpg](https://commons.wikimedia.org/wiki/File:Trader_vic's_queens_park_swizzle.jpg) | Krista | CC BY 2.0 |
| Rob Roy | [Rob Roy Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Rob_Roy_Cocktail.jpg) | TheCulinaryGeek | CC BY 2.0 |
| Rom & Ginger | [Rum and Ginger Beer, New Orleans 2024.jpg](https://commons.wikimedia.org/wiki/File:Rum_and_Ginger_Beer,_New_Orleans_2024.jpg) | Paul Lowry | CC BY 2.0 |
| Rossini | [Un Rossini, grazie (467053126).jpg](https://commons.wikimedia.org/wiki/File:Un_Rossini,_grazie_%28467053126%29.jpg) | Luca Conti from Senigallia, Italy | CC BY 2.0 |
| Roy Rogers | [Roy Rogers Drink.JPG](https://commons.wikimedia.org/wiki/File:Roy_Rogers_Drink.JPG) | Johnl4th | CC BY-SA 3.0 |
| Rum Swizzle | [Rum Swizzle.jpg](https://commons.wikimedia.org/wiki/File:Rum_Swizzle.jpg) | xrayspx | CC BY-SA 2.0 |
| Salted Caramel White Russian | [White Russian - CrystalMixer.jpg](https://commons.wikimedia.org/wiki/File:White_Russian_-_CrystalMixer.jpg) | CrystalMixer - CrystalMixer.com | CC BY 4.0 |
| Salty Caramel Espresso Martini | [Bistrot Bruno Loubet, Clerkenwell, London (4574785649).jpg](https://commons.wikimedia.org/wiki/File:Bistrot_Bruno_Loubet,_Clerkenwell,_London_%284574785649%29.jpg) | Ewan Munro from London, UK | CC BY-SA 2.0 |
| Sambuca con la Mosca | [Flaming Sambuca con la mosca.jpg](https://commons.wikimedia.org/wiki/File:Flaming_Sambuca_con_la_mosca.jpg) | Twentyfour Students from Bangkok, Thailand | CC BY-SA 2.0 |
| Sex on the Beach | [Sex on the beach in Ohrid.jpg](https://commons.wikimedia.org/wiki/File:Sex_on_the_beach_in_Ohrid.jpg) | Sandor Diego Weijn | CC BY 2.0 |
| Shirley Temple | [Canadia-style Shirley Temple.jpg](https://commons.wikimedia.org/wiki/File:Canadia-style_Shirley_Temple.jpg) | Ryan Forsythe (fweez) | CC BY-SA 2.0 |
| Singapore Sling | [Singapore Sling Ingredients.JPG](https://commons.wikimedia.org/wiki/File:Singapore_Sling_Ingredients.JPG) | Achim Schleuning (E-Mail: comander02_de@yahoo.de) | CC BY-SA 4.0 |
| Slippery Nipple | [Slippery Nipple.jpg](https://commons.wikimedia.org/wiki/File:Slippery_Nipple.jpg) | Squelle | Public domain |
| Spicy Margarita | [Prickly Pear Spicy Margarita - January 2024 - Sarah Stierch 02.jpg](https://commons.wikimedia.org/wiki/File:Prickly_Pear_Spicy_Margarita_-_January_2024_-_Sarah_Stierch_02.jpg) | Missvain | CC BY 4.0 |
| Strawberry Margarita | [Margarita de fresa, Mazatlán, 23 de noviembre de 2022.jpg](https://commons.wikimedia.org/wiki/File:Margarita_de_fresa,_Mazatlán,_23_de_noviembre_de_2022.jpg) | El Nuevo Doge | CC0 |
| Tequila Shot | [Tequila shots.jpg](https://commons.wikimedia.org/wiki/File:Tequila_shots.jpg) | Prayitno | CC BY 2.0 |
| Tequila Tonic | [Tequila & Tonic.jpg](https://commons.wikimedia.org/wiki/File:Tequila_&_Tonic.jpg) | Surv1v4l1st | CC BY-SA 3.0 |
| Ti' Punch | [Ti-punch 009.jpg](https://commons.wikimedia.org/wiki/File:Ti-punch_009.jpg) | Arnaud 25 | CC BY-SA 4.0 |
| Tinto de Verano | [Tinto de Verano 2.jpg](https://commons.wikimedia.org/wiki/File:Tinto_de_Verano_2.jpg) | Xemenendura | CC BY-SA 4.0 |
| Tommy's Margarita | [TommysMargarita.jpg](https://commons.wikimedia.org/wiki/File:TommysMargarita.jpg) | Rick Audet | CC BY 2.0 |
| Toronto | [The Toronto Cocktail (13570423424).jpg](https://commons.wikimedia.org/wiki/File:The_Toronto_Cocktail_%2813570423424%29.jpg) | Farther Along | CC BY 2.0 |
| Trinidad Sour | [VTR - Trinidad Sour (18045674468).jpg](https://commons.wikimedia.org/wiki/File:VTR_-_Trinidad_Sour_%2818045674468%29.jpg) | Edsel Little | CC BY-SA 2.0 |
| Tropisk Punch | [Pineapple Gin Punch - Aberdeen Seafood, Brighton 2026-07-19.jpg](https://commons.wikimedia.org/wiki/File:Pineapple_Gin_Punch_-_Aberdeen_Seafood,_Brighton_2026-07-19.jpg) | Andy Li | CC0 |
| Vandmelon Margarita | [Watermelon Margarita or Mojito (14888830500).jpg](https://commons.wikimedia.org/wiki/File:Watermelon_Margarita_or_Mojito_%2814888830500%29.jpg) | Personal Creations | CC BY 2.0 |
| Vieux Carré | [Vieux Carre Cocktail.jpg](https://commons.wikimedia.org/wiki/File:Vieux_Carre_Cocktail.jpg) | Adrian Scottow | CC BY-SA 2.0 |
| Virgin Mary | [Bloody Mary Coctail with celery stalk - Evan Swigart.jpg](https://commons.wikimedia.org/wiki/File:Bloody_Mary_Coctail_with_celery_stalk_-_Evan_Swigart.jpg) | Evan Swigart from Chicago, USA | CC BY 2.0 |
| Ward Eight | [Ward 8 cocktail.jpg](https://commons.wikimedia.org/wiki/File:Ward_8_cocktail.jpg) | CApitol3 (talk)Jim Hood | CC BY-SA 3.0 |
| Woo Woo | [Woo Woo.jpg](https://commons.wikimedia.org/wiki/File:Woo_Woo.jpg) | Stuart Webster from Southampton, England | CC BY 2.0 |
| Æble Fizz | [Grape Spritzer "Mocktail" (20160909-AMS-LSC-9001).jpg](https://commons.wikimedia.org/wiki/File:Grape_Spritzer_"Mocktail"_%2820160909-AMS-LSC-9001%29.jpg) | USDAgov | Public domain |
