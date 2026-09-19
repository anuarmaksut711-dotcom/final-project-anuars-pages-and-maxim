# Pixel Computer Club — design sketches

These text sketches document the intended composition before implementation. They are deliberately simple wireframes rather than replacement graphics.

## Desktop: `index.html`

```text
┌──────────────────────────────────────────────────────────────────────┐
│ Pixel                         About Pixel  Devices & Price  Contact  │ fixed header
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│                    ABOUT PIXEL_                                     │ hero image
│                                                                      │
├──────────────────────────────────────────────────────────────────────┤
│  Pixel Computer Club offers a modern gaming experience...            │ intro
│  More than just a traditional computer club...                       │
├──────────────────────────────────────────────────────────────────────┤
│                         [ large photo ]        Prev / Next           │ CSS slider
├──────────────────────────────────────────────────────────────────────┤
│  [float image]  Pixel brings powerful equipment...                   │ float / clear demo
├──────────────────────────────────────────────────────────────────────┤
│  community copy                                                     │
├──────────────────────────────────────────────────────────────────────┤
│        [photo]        [photo]        [photo]                         │ gallery
│        [photo]        [photo]        [photo]                         │
├──────────────────────────────────────────────────────────────────────┤
│  experience copy                       Pixel Main  @instagram        │ footer/contact
└──────────────────────────────────────────────────────────────────────┘
                                  [Contact]                            │ fixed shortcut
```

## Desktop: `all-locations.html`

```text
┌──────────────────────────────────────────────────────────────────────┐
│ Pixel                         About Pixel  Devices & Price  Contact  │ header
├──────────────────────────────────────────────────────────────────────┤
│                    THE DEVICES AND PRICE_                            │ hero
├──────────────────────────────────────────────────────────────────────┤
│                              PRICES                                   │
│  Packages       Standard             Duo                VIP            │ responsive table
│  1 hour           900                1000              1500           │
│  2 hours         2100                2300              3500           │
│  ...                                                                  │
│               Women receive a 25% discount...                        │ note
├──────────────────────────────────────────────────────────────────────┤
│                              DEVICES                                 │
│       Standard                 Duo                    VIP              │
│       hardware                 hardware               hardware         │ cards
├──────────────────────────────────────────────────────────────────────┤
│  Pixel Main / address                 @instagram / operates 24/7      │ footer
└──────────────────────────────────────────────────────────────────────┘
```

## Mobile behavior

```text
┌──────────────────────┐
│ Pixel          [☰]   │ native details menu
├──────────────────────┤
│ ABOUT PIXEL_         │ hero scales down
├──────────────────────┤
│ text                 │ one readable column
│ [photo]              │ slider keeps the controls visible
├──────────────────────┤
│ gallery item         │ gallery becomes one column
│ gallery item         │
├──────────────────────┤
│ footer items stack   │ footer flex-wrap/column layout
└──────────────────────┘
```

The layout uses the black, purple, lilac, light-lilac and white palette declared in `css/base.css`. Widths, gaps and menu visibility change through CSS media queries only.
