```metadata
title: 5e24 PHB Style
description: ''
tags:
  - meta:Theme
systems:
  - 5e
renderer: V3
theme: 5ePHB
snippets:
  - name: brew_snippets
    subsnippets:
      - name: example snippet
        gen: >-

          The text between `\snippet title` lines will become a snippet of name
          `title` as this example provides.


          This snippet is accessible in the brew tab, and will be inherited if
          the brew is used as a theme.

```

```css
/* FONT IMPORTS __________________________________________________ */
/* _______________________________________________________________ */

@import url('https://rawcdn.githack.com/Kaiburr-kath-hound/HomebreweryStyles/b8a78e9cc74d925556a6e17b32894be6eb26935a/PHB2024Style.css');

/* _______________________________________________________________ */


:root {
  --Note_Background   : #e8d7c4;
  --Descriptive       : #dae8ed;
  --Light_Gray        : #8e8883;
  --Gray              : #67665f;
  --New_Gold          : #d3b885;
  --New_Dark_Red      : #6f1f11;

	--Table_Color_White : #f4f9fa;
	--Table_Color_Blue  : #dae8ed;
  
  --MonsterBackground     : #f4f0eb;
  --Monster_Table_Yellow  : #e8e2d6;
  --Monster_Table_Red     : #d9d0ca;
  --Monster_Table_Green   : #d2d6ce;
  --Monster_Table_Purple  : #cbc6c8;
}

.page {
  /* PAGE TEXTURE */
  background-image    : url(https://ik.imagekit.io/kaiburrkathhound/PageBackground3.jpg);
  
  /* PARAGRAPHS / PLAIN TEXT */
  p {
    line-height       : 1.2em;
  }
  
  /* FOOTER IMAGE */
  &::after {
    height           	: 70px;
    background-image	: url(https://ik.imagekit.io/kaiburrkathhound/Footer.webp);
    opacity           : 0.5;
    z-index           : -2;
  }

  /* HEADERS */
  h1, h2, h3, h4 {
    color             : var(--New_Dark_Red);
  }
  
  h1 {
    + p::first-letter {
      font-size               : 61px;
      font-family             : 'Wolpe Pegasus';
			float                   : left;
			padding-bottom          : 2px;
			padding-left            : 40px;
      padding-right           : 6px;
			margin-top              : -1.8mm;
			margin-bottom           : -20px;
			margin-left             : -40px;
			line-height             : 1em;
      
			color                   : rgba(0, 0, 0, 0);
      background-image        : linear-gradient(#b89956, #d8cdb6);
			-webkit-background-clip : text;
			background-clip         : text;
    }
    
    &::before {
      content           : '';
      position          : relative;
      display           : inline-block;
      margin            :-7.3mm;
      top               : 38px;
      right             : 6px;
      width             : 55px;
      height            : 57px;
      background-size   : 100% 100%;
      background-image  : url('https://ik.imagekit.io/kaiburrkathhound/Symbol.webp');
      z-index           : -1;
      opacity           : 0.7;
    }
    
    /* Makes the first line after an h1 header small-caps */
    + p::first-line {
      font-size       : 116%;
      font-variant    : small-caps;
      letter-spacing  : 0.05mm;
    }
  }
  
  .chapter, .toc, &:has(.frontCover,.insideCover,.frontCredit,.fullPage,.partCover,.backCover) {
    h1::before {
      all   : unset;
    }
  }
  
  h2, h1 {
    letter-spacing  : 1px;
    + p {
      margin-top    : 4px;
    }
  }
  h3 {
    border-bottom   : 2px solid var(--New_Gold); 
  }
  h5 {
    margin-bottom       : -2px;
    -webkit-text-stroke : 0.1px black;
    + table {
      margin-top        : 1px;
    }
  }
  
  /* NOTES */
  .note {
    background-color    : var(--Note_Background);
    padding-top         : 6px;
    border-image				: url(https://ik.imagekit.io/kaiburrkathhound/NoteBorder.webp) 14 stretch;
    border-image-outset	: 6px 0px;
    border-image-width  : 11px;
  }
  
  /* DESCRIPTIVE NOTES */
  .descriptive {
		border-width        : 14px;
		border-image        : url('https://ik.imagekit.io/kaiburrkathhound/DescriptiveBorder.webp') 24 fill stretch;
		border-image-outset : 1px 14px 1px 0px;
    margin              : -3px -7px;
    box-shadow          : unset;
    background-color    : unset;
  }
  
  /* TABLES */
  table:not(.monster table) {
    tbody tr {
      background-color    : var(--Table_Color_White);
      &:nth-child(odd) { 
        background-color  : var(--Table_Color_Blue); 
      }
      td {
        padding   : 0.65mm 1mm;
      }
    }
    thead th {
      padding     : 0.65mm 1mm;
    }
    
     + h5 {
      margin-top  : 23px;
    }
  }
  
  /* SPELL LIST TABLES */
  &:has(.spellList) table {
    th:first-child,
    td:first-child {
      width       : 180px;
    }
  }
  
  
  /* FOOTNOTES & PAGE NUMBERS */
  .footnote, .pageNumber {
    color           :  var(--New_Dark_Red);
    font-family     : 'OPTIPegasus'; 
    font-size       : 14px;
    letter-spacing  : 0.1mm;
    
    &.light {
      color         : var(--New_Gold);
    }
  }
  .footnote {
    font-family     : 'Wolpe Pegasus';
    width           : fit-content;
    text-transform  : lowercase !important;
    font-variant    : small-caps;
    right           : 74px;
    bottom          : 31px;
  }
  .pageNumber {
    right           : 0;
    bottom          : 29px;
  }
  
  /* GRAY HORIZONTAL SEPARATOR */
  &:not(:has(.frontCover,.insideCover,.backCover)) hr {
    visibility        : visible;
    height            : 2.5mm;
    margin            : 4mm 0 2mm;
    background-image  : url(https://ik.imagekit.io/kaiburrkathhound/HorizontalRule.webp);
    background-size   : 100% 100%;
    border            : none;
    opacity           : 0.15;
  }
    
  /* ARTIST CREDITS */
  .artist {
    position          : absolute !important;
    bottom						: 100px;
    width             : 400px;
    left							: 32px;
    transform					: rotate(-90deg);
    transform-origin	: bottom left;
    text-align        : left;
    font-family			  : ScalySansSmallCapsRemake;
    font-size				  : 13px;
    text-transform    : lowercase;
    color							: #999;
  }
  
  /* SMALL CAPS */
  caps {
    font-variant    : small-caps;
    font-size       : 116%;
    letter-spacing  : 0.05mm;
  }
  small {
    position			  : relative;
    text-transform  : lowercase;
    bottom				  : 10px;
    font-size			  : 98%;
  }
  
  /* HYPERLINKS */
  a {
    color						: inherit;
    text-decoration	: none;
    color           : var(--New_Dark_Red);
    font-weight     : bold;
  }
  a:hover{
    text-decoration	: underline;
  }
  
  /* SPACERS - usually for after subclass captions */
  .spacer {
    display         : block;
    margin-bottom   : -6px;
  }

  /* ORIGINS (BACKGROUNDS) */
  .origin {
    --height      : 290px;
    
    display       : block;
    column-span   : all;
    height        : var(--height);
    min-height    : 64px;
    width         : 817px;
    margin-left   : -72px;
    margin-top    : -53px;
 
    img {
      position    : relative;
      min-width   : 817px;
      height      : calc(var(--height) - 22px);
      min-height  : 43px;
      top         : -0;
      left        : -0;
      z-index     : -2;
    }
    
    + h3 {
      position      : relative;
      top           : -54px;
      margin-bottom : -35px;
      font-size     : 23px;
      border        : none;
      text-shadow   : 0 0 3px  rgba(247, 247, 247, 0.5), 
                      0 0 10px rgba(247, 247, 247, 0.8);
      
      &::after {
        content           : '';
        position          : absolute;
        top               : -6px;
        left              : -72px;
        width             : 817px;
        height            : 70px;
        background-size   : 100%;
        background-image  : url('https://ik.imagekit.io/kaiburrkathhound/BackgroundGraphic.webp');
        background-repeat : no-repeat;
        z-index           : -1;
      }
    }
    
    &:not(:first-of-type) {
      margin-top          : 50px;
      background-image    : url('https://ik.imagekit.io/kaiburrkathhound/BackgroundGraphic2.webp');
      background-size     : 100% 10px;
      background-repeat   : no-repeat;
    }
  }
  
  /* FRONT COVER */
  &:has(.frontCover) {
    padding-top : 80px;
    
    img {
      position  : absolute;
    } 

    .logo {
      all                 : unset;
      display             : inline-block;
      width               : 62px;
      height              : 62px;
      margin              : -12px -5px -13px -5px;
      background-image    : url('https://ik.imagekit.io/kaiburrkathhound/HBLogo.webp');
      background-size     : contain;
      background-position : center;
      background-repeat   : no-repeat;
    }

    h3 {
      position        : absolute;
      top             : 43px;
      left            : 0;
      right           : 0;
      font-family     : 'Elan';
      font-size       : 17px;
      letter-spacing  : 1px;
      border          : none;
      color           : red;
    }

    h2 {
      font-family         : 'Elan';
      font-size           : 52px;
      font-weight         : 900;
      -webkit-text-stroke : unset;
      filter              : drop-shadow(0 0 4px black)
                            drop-shadow(0 0 3px rgba(0,0,0,0.7));
      letter-spacing      : 0;
    }

    h1 {
      position            : absolute;
      left                : 0;
      right               : 0;
      top                 : 811px;
      -webkit-text-stroke : 2.5mm black;
      text-shadow         : 0 6px  8px rgba(0,0,0,0.7), 
                            0 6px 12px rgba(0,0,0,0.7);
    }

    &::before {
      content     : '';
      position    : absolute; /* or absolute, depending on your page structure */
      top         : 0;
      left        : 0;
      width       : 100%;
      height      : 100%;
      background  : linear-gradient(to bottom,  rgba(0, 0, 0, 0.9) 0%, 
                                                rgba(0, 0, 0, 0.5) 6%, 
                                                rgba(0, 0, 0, 0) 12%);
      z-index     : 0;
    }
  }
  
  
  /* INSIDE COVER */
  &:has(.insideCover) {
    h1 {
      font-size   : 2.3cm;
      width       : 110%;
      margin-left : -5%;
    }
    hr {
      margin      : 5mm auto;
    }
    .footnote {
      text-align      : center;
      left            : 0;
      right           : 0;
      padding         : 0 50px;
      text-transform  : none;
    }
  }
  
  
  /* CREDITS PAGE */
  &:has(.credits) {
    font-family : ScalySansRemake;
    
    h1::before {
      all       : unset;
    }
  }
  
  
  /* TABLE OF CONTENTS */
  &:has(.toc)::after { 
    display : inherit; 
  }

  .toc {
    h1 {
      text-align  : left;
    }
    a {
      font-weight : 100;
    }
  }
	
  .toc h3,
  .toc h4 {
    font-family			: BookInsanityRemake;
    font-size				: 12px;
    letter-spacing	: 0;
  }

  .toc h3 {
    border-bottom		      : unset;
    
    span:first-of-type {
      -webkit-text-stroke : 1px var(--New_Dark_Red);
    }
  }

  .toc h4 {
    margin-top			: 2px;
    color						: black;
  }

  .toc ul h3 span:first-child::after {
    border-bottom   : 0.05cm dotted #000;
  }

  .toc ul li + li h3 {
    margin-top	    : 8px;
  }

  .toc.wide {
    columns			    : 3;
    column-gap      : 16px;
  }
  
  /* CLASS PAGE */
  .classSymbol img {
    position  : absolute;
    top       : 12px;
    left      : 0;
    right     : 0;
    margin    : auto;
    max-width : 50px;  
  }
  
  &:has(.classTraits) {
    padding-top         : 62px;

    &::before {
      content           : '';
      position          : absolute;
      top               : 12px;
      left              : 7%;
      width             : 86%;
      height            : 550px;
      background-size   : 100% 100%;
      background-image  : url('https://ik.imagekit.io/kaiburrkathhound/ClassBorder.webp');
      z-index           : -1;
    }  

    .classTraits {
      padding-bottom    : 3mm;
      margin-bottom     : 6mm;

      :first-child {
        margin-top  : 2px;
      }

      table {
        margin-top  : 4px;

        tbody tr {
          td {
            padding : 0.65mm 1.5mm;
          }
        }
        thead th {
          padding   : 0.65mm 1.5mm;
        }

        th:first-child,
        td:first-child {
          width     : 140px;
        }
      }
      + p::first-letter {
        font-size               : 57px;
        font-family             : 'Wolpe Pegasus';
        float                   : left;
        padding-bottom          : 2px;
        padding-left            : 40px;
        padding-right           : 6px;
        margin-top              : -1.8mm;
        margin-bottom           : -20px;
        margin-left             : -40px;
        line-height             : 1em;

        color                   : rgba(0, 0, 0, 0);
        background-image        : linear-gradient(#b89956, #d8cdb6);
        -webkit-background-clip : text;
        background-clip         : text;
      }
      + p::first-line {
        font-variant            : small-caps;
        font-size               : 116%;
        letter-spacing          : 0.05mm;
      }

      border-image-slice  : 50;
      border-image-width  : 2.95mm;
      border-image-outset : 0 4.57mm 1.2mm 3.8mm;
      border-image-repeat : stretch stretch;
      border-image-source : url('https://ik.imagekit.io/kaiburrkathhound/ClassTableBorder.webp');
      border-style        : solid;

    }
  }
  
  /* FULL PAGE ART, w/ SUBTITLE */
  &:has(.fullPage) {
    columns         : 1;
    padding-bottom  : 106px;
    display         : flex;
    flex-direction  : column;
    justify-content : flex-end; 
    
    .artist {
      left          : 28px;
      bottom        : 500px;
    }

    h1 {
      margin-bottom : 0;
      font-family   : 'OPTIPegasus';
      font-variant  : small-caps;
      font-size     : 96px;
      text-align    : center;
      letter-spacing: 1px;
      color         : white;      

      -webkit-text-stroke : 6px #656565;
      paint-order         : stroke fill;
      filter              : drop-shadow(0 0 4px rgba(0,0,0,0.4));
    }

    h2 {
      text-align      : center;
      text-shadow     : 1px 2px 3px  rgba(0,0,0,0.7);
      color           : white;
      font-family     : 'TT Jenevers';
      font-size       : 22px;
      font-weight     : 100;
      font-style      : italic;
      letter-spacing  : 0.4px;
    }

    .banner {
      --color           : rgba(177, 154, 120, 0.8);
      padding           : 10px;
      background-image  : linear-gradient(to right, 
                          rgba(0,0,0,0), 
                          var(--color),
                          var(--color), 
                          rgba(0,0,0,0));
      z-index           : 200;
    }
    
    .caption {
      position    : absolute;
      left        : 68px;
      top         : 100px;
      padding     : 3px 5px;
      font-family : 'WalterTurncoat';
      font-size   : 12px;
      width       : fit-content;
      filter      : drop-shadow(0 0 10px black) 
                    drop-shadow(0 0 20px black) 
                    drop-shadow(0 0 10px rgba(0,0,0,0.5));
      color       : white;
      
      p {
        text-indent : 0;
      }

      &.right {
        left  : unset;
        right : 68px;
      }
    }
    
    .fullPage {
      img {
        position    : absolute;
        left        : 50px;
        top         : 30px;
        min-height  : 974px;
        min-width   : 716px;
        z-index     : -4;
        

      }
    }
    &::before {
      content   : '';
      position  : absolute;
      bottom    : 0;
      left      : 0;
      width     : 100%;
      height    : 100%;
      background-image : url('https://ik.imagekit.io/kaiburrkathhound/FullPageBorder.webp');
      background-size : 100% 100%;
      z-index   : -3;
    }
  }
  
  /* HALF PAGE ART */
  &:has(.borderImage) {
    .imageWrapper {    
    --maskWidth   : 332px;
    --maskHeight  : 940px;
    --maskLeft    : 41px;
    --maskTop     : 29px;
    --offsetX     : calc(var(--maskLeft) / 2);
    --offsetY     : calc(var( --maskTop) / 2);
    
    &::before {
      content             : '';
      position            : absolute;
      top                 : var(--maskTop);
      left                : var(--maskLeft);
      width               : max(calc(var(--maskWidth) + 7.6mm), 48mm);
      height              : max(calc(var(--maskHeight) + 7.6mm), 48mm);
      border-image-slice  : 270;
      border-image-width  : 24mm;
      border-image-source : url('https://ik.imagekit.io/kaiburrkathhound/HalfPageBorder.webp');
      z-index             : 1;
    }

    &.leftSide {
      --maskHeight  : 1048px;
      --maskLeft    : 44px;
    }

    &.rightSide {
      --maskHeight  : 1048px;
      --maskLeft    : 417px;
    }

    .borderImage {
      position      : absolute;
      top           : calc(var(--offsetY) + 3.8mm);
      left          : calc(var(--offsetX) + 3.8mm);
      clip-path     : polygon(
        var(--offsetX)                                   calc(var(--offsetY) + 20px), 
        calc(var(--offsetX) + 15px)                      calc(var(--offsetY) + 15px), 
        calc(var(--offsetX) + 20px)                      var(--offsetY), 
        calc(var(--offsetX) + var(--maskWidth) - 20px)   var(--offsetY), 
        calc(var(--offsetX) + var(--maskWidth) - 15px)   calc(var(--offsetY) + 15px), 
        calc(var(--offsetX) + var(--maskWidth))          calc(var(--offsetY) + 20px), 
        calc(var(--offsetX) + var(--maskWidth))          calc(var(--offsetY) + var(--maskHeight) - 20px), 
        calc(var(--offsetX) + var(--maskWidth) - 15px)   calc(var(--offsetY) + var(--maskHeight) - 15px), 
        calc(var(--offsetX) + var(--maskWidth) - 20px)   calc(var(--offsetY) + var(--maskHeight)), 
        calc(var(--offsetX) + 20px)                      calc(var(--offsetY) + var(--maskHeight)), 
        calc(var(--offsetX) + 15px)                      calc(var(--offsetY) + var(--maskHeight) - 15px), 
        var(--offsetX)                                   calc(var(--offsetY) + var(--maskHeight) - 20px)
      );

      img {
        position  : absolute;
        width     : var(--maskWidth);
        height    : max(var(--maskHeight), auto);
        transform : translateY(var(--offsetY))
                    translateX(var(--offsetX));
      }
    }
    
    .caption {
      position    : absolute;
      left        : calc(var(--offsetX) + 50px);
      top         : calc(var(--offsetY) + var(--maskHeight) * 4/5);
      font-family : 'WalterTurncoat';
      font-size   : 12px;
      width       : fit-content;
      max-width   : 314px;
      filter      : drop-shadow(0 0 10px black) 
                    drop-shadow(0 0 15px black) 
                    drop-shadow(0 0 10px rgba(0,0,0,0.5));
      color       : white;

      p {
        text-indent : 0;
      }

      &.rightCaption {
        left    : unset;
        right   : calc(794px - var(--maskWidth) - var(--offsetX));
      }
    }
  }
}

  
  /* CHAPTER HEADERS */
  .chapter {
    --color         : #bc9e5c;
    column-span	    : all;
    display			    : block;
    text-align      : center;
    margin-bottom   : 14px;
    filter          : drop-shadow(0 0 5px white) 
                      drop-shadow(0 0 3px white);
    
    h1 {
      font-family             : 'Wolpe Pegasus';
      font-variant            : small-caps;
      color                   : rgba(0,0,0,0);
			background-image        : linear-gradient(#3d0800, #bb8477 90%);
      background-size         : 100% 1em;
			-webkit-background-clip : text;
      letter-spacing          : 2px;
      font-size               : 54px;
      font-weight             : normal;
      
      /* If you don't like the gray outline in the chapter title, delete the following TWO lines of code */
      -webkit-text-stroke     : 0.25mm #AAA;
      text-stroke             : 0.25mm #AAA;
      
      + h2 {
        margin-top  : -2mm;
      }
    }
    
    hr {
      height            : 25px;
      left              : 0;
      right             : 0;
      margin-top        : 0;
      background-size   : 100% 100%;
      background-image  : url('https://ik.imagekit.io/kaiburrkathhound/ChapterBottom.webp');
      opacity           : 1;
    }
    &.gradient hr::after {
      content             : '';
      position            : absolute;
      width               : 90%;
      height              : 100%;
      left                : 0;
      right               : 0;
      margin              : auto;
      bottom              : 7.8mm;
      -webkit-mask-image  : url('https://ik.imagekit.io/kaiburrkathhound/Gradient.webp');
      -webkit-mask-size   : 100% 100%;
      background-color    : hsl(from var(--color) 
                 /* hue */  h
          /* saturation */  max(calc(s / 2), 30)
           /* lightness */  clamp(30, calc(l * 0.75), 70));
      opacity             : 20%;
      z-index             : -1;
    }
    
    h2 {
      margin-top          : -20px;
      font-family         : 'Wolpe Pegasus';
      font-size           : 28px;
      font-variant        : small-caps;
      font-weight         : 100;
      letter-spacing      : 2px;
      display             : inline-flex;
      align-items         : center;
      color               : hsl(from var(--color) 
                   /* hue */  h 
            /* saturation */  s
             /* lightness */  clamp(40, l, 60));
      
      &::before, &::after {
        content           : '';
        display           : inline-block;
        width             : 118px;
        height            : 38px;
        background-size   : 100% 100%;
      }
      &::before {
        background-image  : url('https://ik.imagekit.io/kaiburrkathhound/Left.webp');
        margin-right      : 4px;
      }
      &::after {
        background-image  : url('https://ik.imagekit.io/kaiburrkathhound/Right.webp');
        margin-left       : 4px;
      }
    }
    
    + p::first-letter {
      font-size               : 61px;
      font-family             : 'Wolpe Pegasus';
			float                   : left;
			padding-bottom          : 2px;
			padding-left            : 40px;
      padding-right           : 6px;
			margin-top              : -1.8mm;
			margin-bottom           : -20px;
			margin-left             : -40px;
			line-height             : 1em;
      
			color                   : rgba(0, 0, 0, 0);
      background-image        : linear-gradient(#b89956, #d8cdb6);
			-webkit-background-clip : text;
			background-clip         : text;
    }
    
    /* Yellow Symbol for Drop Cap */
    &::after {
      content           : '';
      position          : absolute;
      bottom            : -62px;
      left              : -32px;
      width             : 55px;
      height            : 57px;
      background-size   : 100% 100%;
      background-image  : url('https://ik.imagekit.io/kaiburrkathhound/Symbol.webp');
      z-index           : -1;
      opacity           : 0.7;
    }
    
    /* Makes the first line after an h1 header small-caps */
    + p::first-line {
      font-size       : 116%;
      font-variant    : small-caps;
      letter-spacing  : 0.05mm;
    }  
    
    /* Removes all the drop cap formatting if you add "noCap" to the class */
    &.noCap + p::first-letter, &.noCap + p::first-line, &.noCap::after {
        all : unset;
    }
  }
  

  /* MONSTER STATBLOCKS */
  /* ________________________________________________________ */
  /*                                                          */
  /******** Below is an iteration of u/Gambatte's code ------ */
  /* ________________________________________________________ */
  
  .monster {
  font-size             : 3.58mm;
  
    &.frame {
      padding           : 8px 7px;
      background-image  : none;
      background-color  : var(--MonsterBackground);
      border-image      : none;
      border            : 3px double var(--Light_Gray);
      border-radius     : 10px;
      box-shadow        : 3px 3px 5px -2px rgba(136, 136, 136, 0.6);
      margin            : 0 -6px;
      width             : calc(100% + 12px);
    }
    &.wide {
      h2 + p {
        column-span : all;
        margin-bottom : 0.5mm;
      }
    }

    h2 {
      column-span         : all;    
      margin-bottom       : 3px;
      font-family         : 'ScalySansSmallCapsRemake';
      font-size           : 5.4mm;
      letter-spacing      : -0.15mm;
      border-bottom       : 0.35mm solid var(--New_Dark_Red);
      line-height         : 0.9em;
      color               : var(--New_Dark_Red);
      -webkit-text-stroke : 0.1px var(--New_Dark_Red);

      + p {
        color         : var(--Gray);
        font-size     : inherit;
        line-height   : 0.8em;
        margin-bottom : 2.3mm;
      }
    }

    h3 {
      line-height   : 0.9em;
      border-bottom : 0.35mm solid var(--New_Dark_Red);

      &:first-of-type {
        margin-top  : 11px;
      }
      ~ dl {
        color       : inherit;
        line-height : 1.2em;
      }
    }
    
    p {
      + h3 {
        margin-top  : 2.8mm; }
      + p {
        text-indent : 0;
        padding-top : 1.8mm; }
    }

    dl {
      color       : var(--HB_Color_HeaderText);
      line-height : 1.12em;
      
      + dl {
        position  : absolute;
        top       : 44px;
        right     : 50px;
      }
    }
    
    .legend {
      margin-top      : 1mm;
      padding-bottom  : 1.8mm;
      font-style      : italic;
      line-height     : 1.1em;
      color           : var(--Gray);
    }
    
    
    /* MONSTER TABLE */
    table {
      margin      : 2px 0;
      font-size   : 3.4mm;
      
      tbody tr:nth-child(odd) {
        background-color  : unset;
      }
    }

    th {
      color         : var(--Gray) !important;
      font-weight   : normal;
      font-size     : 8px;
      line-height   : 0.8em;
    }

    tr td {
      padding       : 0.3mm 0.5mm;
      border        : solid white; 
      border-width  : 1px 0;
      text-align    : center;
      color         : var(--HB_Color_HeaderText);
      
      &:nth-of-type(4n+1) {
        font-weight   : bold;
        font-variant  : small-caps;
      }
      &:nth-of-type(4n+2) {
        width       : 8%;
      }
      &:nth-of-type(4n+4) {
        width       : 10%;
      }
      
      &:nth-of-type(4), &:nth-of-type(8) {
        clip-path     : polygon(-1px 0, 90% 0, 90% 100%, -1px 100%);
        padding-right : 1.5mm;
        width         : 100px;
      }
      &:nth-of-type(5), &:nth-of-type(9) {
        clip-path     : polygon(10% 0, 102% 0, 102% 100%, 10% 100%);
        padding-left  : 1.5mm;
      }
    }
        
    tr:nth-of-type(odd) {
      td:nth-of-type(4n+1), td:nth-of-type(4n+2) {
        background-color  : var(--Monster_Table_Yellow); 
      }
      td:nth-of-type(4n), td:nth-of-type(4n-1) {
        background-color  : var(--Monster_Table_Red); }
      }
    tr:nth-of-type(even) {
      td:nth-of-type(4n+1), td:nth-of-type(4n+2) {
        background-color  : var(--Monster_Table_Green); 
      }
      td:nth-of-type(4n), td:nth-of-type(4n-1) {
        background-color  : var(--Monster_Table_Purple); 
      }
    }
  }


 /* BACK COVER */
  &:has(.backCover) {
    padding-bottom  : 50px;
    display         : flex;
    flex-direction  : column;
    justify-content : flex-end;
    
    .backCover {
      width               : 100%;
      background-image    : url('https://ik.imagekit.io/kaiburrkathhound/BackCoverBackground.webp');
      background-size     : contain;
      background-position : 0 max(var(--height), 70px);
      padding             : 20px;
      width               : 100%;
      color               : white;
    }

    h1 {
      left                : 0;
      right               : 0;
      width               : 700px;
      margin              : 70px auto;
      font-weight         : 100;
      font-size           : 1.65cm;
      -webkit-text-stroke : 1.5mm black;
      paint-order         : stroke;
      color               : white;
    }

    img {
      height    : calc(var(--height) + 110px);
      min-width : 100%;
      width     : auto;
      position  : absolute;
      left      : 0;
      top       : 0;
    }

    p {
      font-family   : 'Copper Penny DTP';
      font-size     : 2.7mm;
      line-height   : 4.4mm;
      width         : 464px;

      + p {
        text-indent : 0;
        padding-top : 16px;
      }
    }

    caps {
      -webkit-text-stroke : 0.1mm white;
    }
    
    .banner {
      --color       : #555557;
      padding       : 3mm 0.16cm;
      padding-left  : 13mm;
      margin-top    : 8mm;
      margin-left   : -13mm;
      background    : linear-gradient(to right, var(--color) 0%, var(--color) 90%, rgba(0, 0, 0, 0) 100%);
      width         : 490px;
      p {
        width       : 390px;
      }
    }
    
    .logo {
      bottom    : max(calc((1156px - var(--height))/2), 2.5cm);
      left      : unset;
      right     : 0mm;
      
      img {
			  height    : 2.3cm;
        min-width : unset;
        width     : 2.3cm;
      }

      hr {
        margin-top    : 6px;
        + * {
          margin-top  : 20px;
        }
      }
      
      a {
        color         : #68686a;
      }

      p {
        font-family   : 'Copper Penny DTP';
        font-variant  : small-caps;
        line-height   : 1em;
        
        color         : #d69d00;
        
        /* The following lines of code restore the "golden" texture for text; delete this line of code (line 1045) as well as line 1050
        color                   : rgba(0,0,0);
			  background-image        : linear-gradient(-45deg, #c9a02c, #f9bf24, #815003, #dfa311);
        -webkit-background-clip : text;
        background-clip         : text;
        */
      }
      
      p:nth-letter(2) { 
        color : red; 
      }
    }
  }
  
  /* EVEN-NUMBERED PAGE DIFFERENCES */
  &:nth-of-type(even) {
    background-position : right;
    
    .footnote {
      left  : 74px;
    }

    .pageNumber {
      left  : 0;
    }

    .artist {
      left						  : 784px;
    }
    &:has(.fullPage) {
      .artist {
        left            : 803px;
      }
    }
  }
}
```

<!---
The class below MUST be included somewhere on your front page for everything on the page to be formatted properly, but it doesn't matter where.
--->
{{frontCover}}

### THE WORLD'S GREATEST RPG DOCUMENT FORMATTER

<!---
The logo class here inserts the homebrewery logo. It's used here instead of the "&" in the D&D logo.
--->
## HOME {{logo}} BREWERY

# Player's Book of Hands

<!---
The "styling" code below is inside the curly brackets {}. Feel free to adjust those to see what changes. 
--->
![Front Cover Image](https://ik.imagekit.io/kaiburrkathhound/PHBCover.jpg) {bottom:-7.4%,left:-416px,height:115%}

\page

<!---
Similar to the front cover, this class MUST be included somewhere to format the page.
--->
{{insideCover}}

# Player's Book of Hands
___
{width:10cm}
<!---
The styling code above changes the width of the red underline, this is actually a formatting technique that I straight up DIDN'T know before making this template. C'est la vie.
--->

![background image](https://ik.imagekit.io/kaiburrkathhound/PHBInsideCover.webp){position:absolute,top:295px,left:175px,width:465px}


<!---
The two following "page stains" are generated using the Homebrewery's Images menu at the top of this editing window (Click IMAGES, then WATERCOLOR SPLATTER). There are 12 different images, denoted by "watercolor1", "watercolor7", etc..
--->
{{watercolor6,top:0px,left:830px,width:320px,transform:rotate(-50deg),background-color:#aaa4bc,opacity:70%}}

{{watercolor2,top:130px,left:-180px,width:410px,transform:rotate(30deg),background-color:#dbc899,opacity:70%}}

<!---
The following code is for giving credit (and providing a link!) to the artist on the inside cover. PLEASE give credit to whatever art you use!! 
--->
{{artist,left:38px
[Daarken](https://www.daarken.com/)
}}

<!---
Speaking of credit, this is the icon for the Homebrewery itself, which is a super cool program that we all get to use for free! Credit where credit is due.
--->
{{logo ![](/assets/naturalCritLogoRed.svg)}}

\page

<!---
The typical style for credits pages includes paragraphs with hanging indents. To use those, make sure to include a double colon : somewhere in the paragraph, and you're all set!
--->
# Credits

**Template Designer:** :: [u/Kaiburr_Kath-Hound](https://www.reddit.com/user/Kaiburr_Kath-Hound/)

Thanks to [u/Gambatte](https://www.reddit.com/user/Gambatte/) for the use of their monster stat block code.

##### Artist Credits
**Front Cover:**  :: *PHB 2024* by [Tyler Jacobson](http://www.tylerjacobsonart.com/)
**Inside Cover:** :: *Unknown*, by [Daarken](https://www.daarken.com/), @Wizards of the Coast 
**Back Cover:**   :: *Unknown*, by [Tyler Jacobson](http://www.tylerjacobsonart.com/), @Wizards of the Coast 


\column


**Page 4**      :: *unknown* by [Dmitri Burmak](https://burmak.ru/), @Wizards of the Coast
**Page 6**      :: *College of Dance* by [Katerina Ladon](https://www.artstation.com/katerina_ladon), @Wizards of the Coast
**Page 9a:**    :: *Acolyte* by [Titus Lunter](https://tituslunter.com/), @Wizards of the Coast
**Page 9b:**    :: *Artisan Studio* by [Luca Bancone](https://www.artstation.com/lucabancone), @Wizards of the Coast

<!---
The .wide class can be used for a lot of different things. This one here basically separates the top half of the page and the bottom half, that way the two "frontCredits" with images can be placed precisely next to one another, regardless of the content on the top of the page.
--->
{{wide}}

<!---
The front cover credits use the new image 2024 frame, which is detailed later in thie document!
--->
{{imageWrapper,--maskWidth:310px,--maskHeight:210px,--maskLeft:64px,--maskTop:255px
{{borderImage ![front cover](https://ik.imagekit.io/kaiburrkathhound/PHBCover.jpg) {top:-20px,left:0px} }}
}}

##### On the Cover
{margin-top:230px}
Guided by a gold dragon, the elf queen Yolande and the heroes of Valor's Call test their bravery against evil in this daring scene illustrated by [Tyler Jacobson](https://www.tylerjacobsonart.com/).

\column


{{imageWrapper,--maskWidth:306px,--maskHeight:210px,--maskLeft:417px,--maskTop:255px
{{borderImage ![alt cover](https://ik.imagekit.io/kaiburrkathhound/AltCover.jpeg) {top:0px,left:0px} }} 
}}

##### On the Alt-Cover
{margin-top:230px}
Nothing's Better than sharing stories with friends. Heroes pause to share tea and tales with a gold dragon in this serene illustration by [Wylie Beckert](https://www.wyliebeckert.com/).

<!---
The following text is what must be included on free content using the 5e 2014 rules. Technically we're not sure what the requirements will be for content relating to 5e 2024, but I included it here to be safe. 

Wizards of the Coast (who own D&D) is typically very accommodating to D&D creators who release original content for free (although there is one very specific, very public time where they were NOT chill; fingers crossed that doesn't happen again).
--->
{{footnote
The contents of this document is unofficial Fan Content permitted under the Fan Content Policy. Not approved/endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast. ©Wizards of the Coast LLC.
}}

{{credits}}

\page

<!---
The Table of Contents can be automagically generated using the TEXT EDITOR menu, then TABLE OF CONTENTS buttons at the top of this editor window. The table below was generated that way, with only some minor adjustments.
--->
{{toc,wide
# Contents

- ### [{{ Playing the Game}}{{ 5}}](#p5)
  - #### [{{ chapter 2}}{{ 6}}](#p6)
- ### [{{ Creating a Character}}{{ 6}}](#p6)
  - #### [{{ Player or DM?}}{{ 6}}](#p6)
    -  [{{ Being a Player}}{{ 6}}](#p6)
    -  [{{ Being the Dungeon Master}}{{ 6}}](#p6)
  - #### [{{ Rhythm of Play}}{{ 6}}](#p6)
  - #### [{{ Bard Subclasses}}{{ 7}}](#p7)
    -  [{{ College of Lorem}}{{ 7}}](#p7)
  - #### [{{ Wizard}}{{ 8}}](#p8)
    -  [{{ Becoming a Wizard…}}{{ 8}}](#p8)
    -  [{{ Wizard Class Features}}{{ 8}}](#p8)
    -  [{{ Wizard Spell List}}{{ 9}}](#p9)
  - #### [{{ Character Origins}}{{ 10}}](#p10)
    -  [{{ Devotee}}{{ 10}}](#p10)
    -  [{{ Crafty-pants}}{{ 10}}](#p10)
}}

\page

<!---
The .fullPage class works a little differently now; there is a static ":before" image that frames whatever iumage you place "behind" it, allowing you to independently control how large and where the image is, without affecting the border itself.

NOTE: the halfPage image class does NOT work like this, and you cannot move the image mask and the image around independently in the halfPage class.
--->
{{fullPage

![image](https://ik.imagekit.io/kaiburrkathhound/FullpageArt.jpeg) {width:950px,left:-45px;}

}}

<!---
The caption here can be placed on the left or right, provided you specify which side using the .left or .right tags. The default vertical placement is 50 pixels down from the top of the frame, but can be changed by adding ",top:350px" (or any other value).
--->
{{caption,right
World-traveling explorers Hank, Bobby, 

Sheila, Diana, and Presto stand on the 

threshold of their next adventure
}}

# Playing the Game


<!---
The banner requires a special color input, called "RGBA" (Red, Green, Blue, Alpha). The three color values go from 0 to 255. 'Alpha' just means opacity, from a scale of 0 (transparent) to 1 (opaque). 

https://www.hexcolortool.com/ is an excellent tool for selecting this type of color, just use the sliders to select the desired color, and look for the generated "rgba" values. 

I highly recommend an alpha value between 0.7 to 0.9

Below is the default colored banner from the PHB. If you leave it blank, the default color will still be shown.
--->
{{banner,--color:"rgba(177, 154, 120, 0.8)"
## A List of Rules to... Read, I guess
}}

<!---
The artist's credit is still visible on these pages! Seriously, always give credit to the artist.
--->
{{artist
[Dmitri Burmak](https://burmak.ru/)
}}

{{pageNumber,auto}}
\page

<!---
The .chapter class here is cool, and flexible for whether the h1 or h2 header is included, what order they're in, etc.

If you want to forgo the gradient background, just delete "gradient", and if you want to forgo the drop cap formatting (the first big letter after the chapter), just add ",noCap" to the end of the line.

The main thing here is that the h2 header (the small one) and the gradient colors are linked, and can both be changed entirely by changing the --color value. Visit www.hexcolortool.com to pick a color with a usable hexadecimal code. Below are the (approximate) color values in the actual PHB.
--->

<!---
PHB Color values by chapter:

- Intro/Index (Yellow)      : #b39a59
- Chapter 1 (Pink-red)      : #9a4835
- Chapter 2 (Green)         : #676b36
- Chapter 3 (Red-Orange)    : #a74d3a
- Chapter 4 (Light Blue)    : #8a86b2
- Chapter 5 (Dark Red)      : #7c4848
- Chapter 6 (Cyan)          : #5fa7a1
- Chapter 7 (Mauve)         : #9a677b

- Appendix A (Light Purple) : #a092a0
- Appendix B (Nat Yellow)   : #c0b797
- Appendix C (Yellow)       : #b39a59 
--->

{{chapter,gradient,--color:#7c4848

## chapter 2
# Creating a Character
___
}}

Imagination is a key ingredient of <caps>Dungeons & Dragons</caps>, a cooperative game in which the characters that you roleplay embark on adventures together in fantasy worlds filled with monsters and magic.

In D&D, the action takes place in the imaginations of the players, and it’s narrated by everyone together.

{{note
##### Rules Glossary
If you read a rules term in this book and want to know its definition, consult the rules glossary, which is appendix C. This chapter provides an overview of how to play D&D and focuses on the big picture. Many places in this chapter reference that glossary.
}}

## Player or DM?
To play D&D, you need one person to be the Dungeon Master and other players (three to six are best) to play adventurers. Which role is right for you?

### Being a Player
If you want to be one of the protagonists in your group’s adventures, consider being a player. Here’s what players do:

**Make a Character.** :: Your character is your alter ego in the fantasy world of the game. After you read this chapter, use the rules in chapter 2 to create your character.

<!---
The three underscores below form the gray-bar separator, and are used in lots of different parts of the 2024 books. It technically isn't used in THIS part of the DMG, but I added it anyway. You don't own me.
--->
___


<!---
Similarly, the descriptive text block is not used here in the 2024 DMG, but this element is modeled after the first 2024 D&D adventure "Uni and the Hunt for the Lost Horn".
--->
{{descriptive
**Team Up.**          :: Your character joins the other players’ characters to form an adventuring party. These adventurers are allies who face challenges and fantastical situations together. Each character brings distinctive capabilities, which ideally complement those of the other characters.
**Venture Forth.**    :: Your character’s group explores locations and events presented by the DM. You can respond to them in any way you can imagine, guided by the rules in this book. Although the DM controls all the monsters you encounter, the DM isn’t your adversary. The DM guides your party’s journey as your characters become more powerful.
}}


\column



##### Character Advancement
| Experience Points | Level | Proficiency Bonus |
|:------------------|:-----:|:-----------------:|
| 0                 | 1     | +2                |
| 300               | 2     | +2                |
| 900               | 3     | +2                |
| 2,700             | 4     | +2                |
| 6,500             | 5     | +3                |
| 14,000            | 6     | +3                |

<!---
A small thing, but when a colon appears on its own line, it becomes a vertical spacer to separate different elements. More colons, more vertical space.
--->
::

<!---
This is an updated version of the new monster stat block after I got a closer look at the formatting. 

NOTE: The Homebrewery Monster Stat Block generator button above (PHB menu, then MONSTER STAT BLOCK) will NOT work to make the "new" version of the stat block; I recommend copying the following stat block and modifying it to match your monster:
--->
{{monster,frame
## Mind Ferret
*Tiny guy, narrow-minded neutral*

**AC**         :: 15 (Chain shirt)
**HP**         :: 120 (48d4)
**Speed**      :: 45 ft.

**Initiative** :: +2 (12)

|   |   | MOD | SAVE |   |   | MOD | SAVE |   |   | MOD | SAVE |
|:--|:-:|:---:|:----:|:--|:-:|:---:|:----:|:--|:-:|:---:|:----:|
|Str| 20|  +5 |  +5  |Dex| 14|  +2 |  +2  |Con| 11|  +0 |  +0  |
|Int|  9| --1 | --1  |Wis|  7| --2 | --2  |Cha| 30| +10 | +10  |

**Immunities**  :: Drunk, Groovy
**Senses**      :: Darkvision 6,000 ft., Passive Perception 12
**Languages**   :: None, but it can read vibes
**CR**          :: 15 (XP 2043; PB +5)

### Traits
***Onion Stench.*** Any creatures within 5 feet of this thing develops an irrational craving for onion rings.

***Pack Tic Tacs.*** These guys ALWAYS have Tic Tacs.

### Actions
***Airplane Hammer.*** *Melee Weapon Attack:* +4, reach 5 ft. *Hit:* 5 (1d6 + 2) Bludgeoning damage.

### Legendary Actions
{{legend Legendary Action Uses: 3 (4 in Lair). Immediately after another creature's turn, the ferret can expend a use to ake one of the following actions. The ferret regains expended uses at the start of each of its turns.}}

***Hammer Time.*** The ferret makes akes two Airplane Hammer attacks.

***Nervous Tic.*** The ferret consumes one of its Tic Tacs, regaining 20 hit points.

}}

<!---
Below is how you denote the page number and footer text. If you want to manually enter the page number, replace the ",auto" with a space, then whatever number you want.
--->
{{pageNumber,auto}}
{{footnote Chapter 2 | Creating a Character}}
\page

<!---
Here's the newest update for the gold-bordered images. This version DOES allow you to format the image and the border separately. The border is determined by the following 4 variables:
  --maskWidth
  --maskHeight
  --maskLeft
  --maskBottom

Alternatively, if you want to have the image to take up the entirety of the left or righthand side of the page, you can simply add 'leftSide' or 'rightSide' tag to the 'imageWrapper' class below, and the image will automatically format itself to the PHB subclass proportions.
--->
{{imageWrapper,--maskWidth:332px,--maskHeight:1048px,--maskLeft:41px,--maskTop:29px

{{borderImage ![dance background](https://ik.imagekit.io/kaiburrkathhound/BardArt.jpeg) {top:0px,left:0px} }} 

<!---
The caption can be formatted on the left or right side of the image (by using the 'rightCaption' tag), similar to the image itself, and defaults to being 80 pixels off the bottom of the page, but can be adjusted.
--->
{{caption,rightCaption
College of Dance <br> Subclass
}}

}}

<!---
This is an overlaid image, to give the illusion that it's "popping out" of the frame. This is really hard to do without Photoshop (or my favorite free alternative, www.photopea.com).
--->
![dance overlay](https://ik.imagekit.io/kaiburrkathhound/Img3.webp) {position:absolute,top:465px,left:11px,width:125px,z-index:1}

<!---
This gives credit in the same way as before, and appears on the left or right hand side of the page, depending on whether the page number is odd or even.
--->
{{artist
[Katerina Ladon](https://www.artstation.com/katerina_ladon)
}}

<!---
This code lets you manually place the column break in the page. Since the bard image takes up the entire vertical area on the left side of the page, all the text has to appear on the right side.
--->
\column

<!---
BTW, since the Dance Bard is not part of the free released rules the content here is all "lorem ipsum" generated text.
--->
## Bard Subclasses
Ipsum venenatis conubia blandit faucibus tempus ad ex ligula. In ultrices nascetur nascetur suscipit venenatis mauris faucibus pharetra. Aliquam parturient ipsum id vel magna. Placerat mollis nostra quisque pretium eros nulla nibh. This section presents the College of Lorem, College of Ipsum, College of Dolor, and College of Bit Subclasses.

### College of Lorem
*Dolor Sit Amet Consectetur*

<!---
This is a really small class, and ONLY provides a tiny vertical space (less than a colon symbol would)
--->
{{spacer}}

Bards of the College of Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Fusce montes aliquet leo nullam inceptos class urna velit.

#### Level 3: Ipsum Vivamus
Nulla aliquet enim tortor, at auctor quam tincidunt necFusce montes aliquet leo class urna velit:

***Luctus Aliquam.*** Et tortor risus curabitur nullam lacinia. Justo magna fringilla fusce ex ipsum nisl phasellus lobortis. 

***Curabitur Aliquet.*** Pellentesque in ipsum id orci porta dapibus. Curabitur aliquet quam id dui  blandit.

***Vivamus Blandit.*** Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a, eget urna convallis. Non nunc gravida hendrerit; nulla feugiat natoque per. Dui conubia enim maecenas lobortis quis consequat.

***Euismod Nisi.*** In egestas erat imperdiet sed euismod nisi porta lorem mollis. Donec sollicitudin molestie malesuada. Sed viverra ipsum nunc aliquet bibendum enim facilisis gravida neque convallis a. Nullam vehicula ipsum a arcu cursus. Sed viverra ipsum nunc aliquet bibendum enim facilisis gravida neque convallis a iaculis id justo. At litora congue vel mollis orci platea.

#### Level 6: Congue Dictum
Donec sollicitudin molestie malesuada. Nulla porttitor accumsan tincidunt, lorem ipsum dolor sit amet consectetur adipiscing elit.  Sed cras ornare arcu dui vivamus arcu felis. Nisl aptent tincidunt ipsum, scelerisque ultricies nam! Quam nam laoreet tempus arcu ac hendrerit.

Vitae Ipsum. Phasellus vehicula velit ut tortor pretium viverra suspendisse potenti.

#### Level 6: Vulputate Ligula
Pellentesque in ipsum id orci porta dapibus. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Quis enim lobortis scelerisque fermentum dui faucibus. Egestas tellus rutrum tellus pellentesque. Nisl aptent tincidunt ipsum, scelerisque ultricies nam! Quam nam laoreet tempus arcu ac hendrerit.

{{pageNumber,auto}}
{{footnote Chapter 3 | Character Classes}}
\page

<!---
The class page is for making your own classes, obviously, and is formatted based on whether the .classTraits class appears on the page.

The .classSymbol class below formats the image inside it to be inside the little crest at the top of the page. The image shown is the Homebrewery logo. 

If you want to make your own class symbol, the color used for the frame and this example image is #caac76.
--->
{{classSymbol ![](https://ik.imagekit.io/kaiburrkathhound/ClassSymbol.webp) {width:40px,margin-top:5px} }}

<!---
Pretty self explanatory, but this class' frame will extend or retract depending on how big the .classTraits table is.
--->
{{classTraits
##### Core Wizard Traits
|                                |                         |
|:-------------------------------|:------------------------|
| **Primary Ability**            | Intelligence            |
| **Hit Point Die**              | D6 per Wizard level     |
| **Saving Throw Proficiencies** | Intelligence and Wisdom |
| **Skill Proficiencies**        | *Choose 2:* Arcana, History, Insight, Investigation, Medi- cine, Nature, or Religion |
| **Weapon Proficiencies**       | Simple weapons          |
| **Armor Training**             | None                    |
| **Starting Equipment**         | *Choose A or B:* (A) Leather Armor, 2 Daggers, Shortsword, Shortbow, 20 Arrows, Quiver, Thieves’ Tools, Burglar’s Pack, and 8 GP; or (B) 100 GP |
}}

Wizards are defined by their exhaustive study of magic’s inner work- ings. They cast spells of explosive fire, arcing lightning, subtle deception, and spectacular transformations. Their magic conjures monsters from other planes of existence, glimpses the future, or forms protective barriers. Their mightiest spells change one substance into another, call meteors from the sky, or open portals to other worlds.

Most Wizards share a scholarly approach to magic. They examine the theoretical underpinnings of magic, particularly the categorization of spells into schools of magic. Renowned Wizards such as Bigby, Tasha, Mordenkainen, and Yolande have built on their studies to invent iconic spells now used across the multiverse.

The closest a Wizard is likely to come to an or- dinary life is working as a sage or lecturer. Other Wizards sell their services as advisers, serve in mili- tary forces, or pursue lives of crime or domination.

But the lure of knowledge calls even the most unadventurous Wizards from the safety of their libraries and laboratories and into crumbling ru- <br>ins and lost cities. Most Wizards believe that their counterparts in ancient civilizations knew secrets of magic that have been lost to the ages, and discov- ering those secrets could unlock the path to a power greater than any magic available in the present age.

<!---
All the content on this page was released in the free D&D 2024 rules, found here:
https://www.dndbeyond.com/sources/dnd/free-rules/character-classes
--->
### Becoming a Wizard...
#### As a Level 1 Character
- Gain all the traits in the Core Wizard Traits table.
- Gain the Wizard’s level 1 features, which are listed in the Wizard Features table.

\column

#### As a Multiclass Character
- Gain the Hit Point Die from the Core Wizard Traits table.
- Gain the Wizard’s level 1 features, which are listed in the Wizard Features table. See the multiclassing rules in chapter 2 to determine your available spell slots.

### Wizard Class Features
As a Wizard, you gain the following class features when you reach the specified Wizard levels. These features are listed in the Wizard Features table.

#### Level 1: Spellcasting
As a student of arcane magic, you have learned to cast spells. See chapter 7 for the rules on spellcasting. The information below details how you use those rules with Wizard spells, which appear in the Wizard spell list later in the class’s description.

<!---
In case you haven't seen this notation before, the asterisks on the line below denote both *italicized* text (one asterisk on each side of the affected text) AND **bold** text (two asterisks on each side).
--->
***Cantrips.*** You know three Wizard cantrips of your choice. Light, Mage Hand, and Ray of Frost are recommended. Whenever you finish a Long Rest, you can replace one of your cantrips from this feature with another Wizard cantrip of your choice.

When you reach Wizard levels 4 and 10, you learn another Wizard cantrip of your choice, as shown in the Cantrips column of the Wizard Features table.

***Spellbook.*** Your wizardly apprenticeship culminated in the creation of a unique book: your spellbook. It is a Tiny object that weighs 3 pounds, contains 100 pages, and can be read only by you or someone casting Identify. You determine the book’s appearance and materials, such as a gilt-edged tome or a collection of vellum bound with twine.

The book contains the level 1+ spells you know. It starts with six level 1 Wizard spells of your choice. Detect Magic, Feather Fall, Mage Armor, Magic Missile, Sleep, and Thunderwave are recommended.

Whenever you gain a Wizard level after 1, add two Wizard spells of your choice to your spellbook. Each of these spells must be of a level for which you have spell slots, as shown in the Wizard Features table. The spells are the culmination of arcane research you do regularly.

***Spell Slots.*** The Wizard Features table shows how many spell slots you have to cast your level 1+ spells. You regain all expended slots when you finish a Long Rest.

***Prepared Spells of Level 1+.*** You prepare the list of level 1+ spells that are available for you to cast with this feature. To do so, choose four spells from your spellbook. The chosen spells must be of a level for which you have spell slots.

{{pageNumber,auto}}
{{footnote chapter 3 | character classes}}
\page

### Wizard Spell List
This section presents the Wizard spell list. The spells are organized by spell level and then alphabetized, and each spell’s school of magic is listed. In the Special column, *C* means the spell requires Concentration, *R* means it’s a Ritual, and *M* means it requires a specific Material component.

<!---
The .spellList class has only one unique trait, in that any table on the same page as that class will have the same width for their first columns, instead of the columns being dynamic based on the content. 

If this wasn't the case, then all the tables look kind of wonky when they're on the same page.
--->
{{spellList}}

##### Cantrips (Level 0 Wizard Spells)
|  Spell             | School        | Special |
|:-------------------|:--------------|:-------:|
| *Acid Splash*      | Evocation     | —       |
| *Chill Touch*      | Necromancy    | —       |
| *Dancing Lights*   | Illusion      | C       |
| *Fire Bolt*        | Evocation     | —       |
| *Light*            | Evocation     | —       |
| *Mage Hand*        | Conjuration   | —       |
| *Mending*          | Transmutation | —       |
| *Message*          | Transmutation | —       |
| *Minor Illusion*   | Illusion      | —       |
| *Poison Spray*     | Necromancy    | —       |
| *Prestidigitation* | Transmutation | —       |
| *Ray of Frost*     | Evocation     | —       |
| *Shocking Grasp*   | Evocation     | —       |
| *Thunderclap*      | Evocation     | —       |
| *True Strike*      | Divination    | —       |

##### Level 1 Wizard Spells
| Spell                           | School        | Special |
|:--------------------------------|:--------------|:-------:|
| *Alarm*                         | Abjuration    | R       |
| *Burning Hands*                 | Evocation     | —       |
| *Charm Person*                  | Enchantment   | —       |
| *Color Spray*                   | Illusion      | —       |
| *Comprehend Languages*          | Divination    | R       |
| *Detect Magic*                  | Divination    | C, R    |
| *Disguise Self*                 | Illusion      | —       |
| *Expeditious Retreat*           | Transmutation | C       |
| *False Life*                    | Necromancy    | —       |
| *Feather Fall*                  | Transmutation | —       |
| *Find Familiar*                 | Conjuration   | R, M    |
| *Fog Cloud*                     | Conjuration   | C       |
| *Grease*                        | Conjuration   | —       |
| *Identify*                      | Divination    | R, M    |

\column

| Spell                           | School        | Special |
|:--------------------------------|:--------------|:-------:|
| *Illusory Script*               | Illusion      | R, M    |
| *Jump*                          | Transmutation | —       |
| *Longstrider*                   | Transmutation | —       |
| *Mage Armor*                    | Abjuration    | —       |
| *Magic Missile*                 | Evocation     | —       |
| *Protection from Evil and Good* | Abjuration    | C, M    |
| *Shield*                        | Abjuration    | —       |
| *Silent Image*                  | Illusion      | C       |
| *Sleep*                         | Enchantment   | C       |
| *Thunderwave*                   | Evocation     | —       |
| *Unseen Servant*                | Conjuration   | R       |

##### Level 2 Wizard Spells
| Spell                 | School        | Special |
|:----------------------|:--------------|:-------:|
| *Alter Self*          | Transmutation | C       |
| *Arcane Lock*         | Abjuration    | M       |
| *Augury*              | Divination    | R, M    |
| *Blindness/Deafness*  | Transmutation | —       |
| *Blur*                | Illusion      | C       |
| *Continual Flame*     | Evocation     | M       |
| *Darkness*            | Evocation     | C       |
| *Darkvision*          | Transmutation | —       |
| *Detect Thoughts*     | Divination    | C       |
| *Enhance Ability*     | Transmutation | C       |
| *Enlarge/Reduce*      | Transmutation | C       |
| *Flaming Sphere*      | Evocation     | C       |
| *Gentle Repose*       | Necromancy    | R, M    |
| *Gust of Wind*        | Evocation     | C       |
| *Hold Person*         | Enchantment   | C       |
| *Invisibility*        | Illusion      | C       |
| *Knock*               | Transmutation | —       |
| *Levitate*            | Transmutation | C       |
| *Locate Object*       | Divination    | C       |
| *Magic Mouth*         | Illusion      | R, M    |
| *Magic Weapon*        | Transmutation | —       |
| *Mirror Image*        | Illusion      | —       |
| *Misty Step*          | Conjuration   | —       |
| *Ray of Enfeeblement* | Necromancy    | C       |
| *Rope Trick*          | Transmutation | —       |

{{pageNumber,auto}}
{{footnote chapter 3 | character classes}}
\page

<!---
The .origin class is similar to the halfPage class, where you need to specify a height for the image. Here are all the formatting details:

- The image will always be the height that you specify in the --height variable.
- If the width of the image is WIDER than it is supposed to be based on the current height, the extra width will be "pushed out" to the right of the page.
- If the height of the image is THINNER than it is supposed to be, the image will "squish" to reach the edges of the frame; make the --height value larger to fix this.

Please experiment with the --height values below in order to see what I mean.
--->
{{origin,--height:330px
![acolyte art](https://ik.imagekit.io/kaiburrkathhound/Devotee.jpeg){}
}}

<!---
I made the backgrounds on this page out of Gen Z terms, mostly for fun.
--->
### Devotee
**Ability Scores:**       :: Smarts, Big Brain, Rizz 
**Feat:**                 :: Sparkle Initiate (see Feats)
**Skill Proficiencies:**  :: Vibe Check and Zodiac
**Tool Proficiency:**     :: Calligrapher’s Supplies 
**Equipment:**            :: *Choose A or B:* (A) Calligrapher’s Supplies, Book, Holy drip, 8 GP; or (B) 50 GP

\column

You threw yourself into the temple hustle, highkey hitting that daily grind in a cozy town shrine or a hidden paradise. There, you stanned for either a cheugy deity or a celestial NPC. Your mentor was bussin, gave your brain a glow up, and let you flex your magics to make straight vibes.

<!---
Note: Specifying the bottom placement value makes the artist credit more visible 
--->
{{artist,bottom:630px [Titus Lunter](https://tituslunter.com/)}}

<!---
You can place multiple origin classes on the same page, and each subsequent class should have that golden double-line at the top of every image except for the first.
--->
{{origin,--height:319px
![artisan art](https://ik.imagekit.io/kaiburrkathhound/CraftyPants.jpeg){}
}}

### Crafty-pants
**Ability Scores:**       :: Swole, Zoom-zoom, Big Brain 
**Feat:**                 :: Vape Supplier (see Feats)
**Skill Proficiencies:**  :: Snoop and Rizz Up
**Tool Proficiency:**     :: *Choose one kind of Crafty-Pants' tools* (see chapter 6)
**Equipment:**            :: *Choose A or B:* (A) Crafty-Pants' tools (same as above), 2 Vape Pouches, Normie Clothes, <br>32 GP; or (B) 50 GP

\column

You started wiping down counters in your blue collar era for like, literal pennies (big oof). Fast forward, you leveled up to apprentice status, ate that basic craftwork (no crumbs), and lowkey mastered the art of rizzing up those customers; Speech 100. And now, thanks to the grind, your detail work is straight fire, no cap.

{{artist,bottom:120px [Luca Bancone](https://www.artstation.com/lucabancone)}}

{{pageNumber,auto}}
{{footnote chapter 4 | character origins}}
\page

<!---
The back cover page, like many classes in this template, uses a --height variable to format everything properly. This value affects both the height of the background image and the height of the black border at the bottom of the page.

The sweet spot for the --height value is to make the transition between the image and the border to be RIGHT in between the h1 header and the first paragraph.
--->
{{--height:708px

<!---
Like before, just include this class somewhere on the page.
--->
{{backCover}}

<!---
Images will format themselves to fill the space, but you can add any styling code you want between the curly brackets.
--->
![background image](https://ik.imagekit.io/kaiburrkathhound/BackCover.jpeg){}

# Create Heroic Characters

<!---
This paragraph includes the "<caps>" class. This is mostly to emulate the weird thing that D&D books do, where they make the trademarked terms "D&D" and "Dungeons & Dragons" appear in small-caps formatting.

It's very odd, and not likely that you'll need to use this formatting, but it's here just to show it as an option.
--->
This revised and expanded *Player's Book of Hands* is the essential reference for every fifth edition <caps>Dungeons & Dragons</caps> player. It contains rules for character creation and advancement, exploration, combat, equipment, spells, and much more.

Create fantastic <caps>D&D</caps> heroes from the wide selection of character origins, classes, and subclasses provided. Explore ancient ruins and deadly dungeons. Battle monsters while searching for legendary treasures. Gain experience and power as you trek across uncharted lands with your companions

<!---
The PHB used this banner to show the D&D logo and to declare what other books are releasing in the base game. I'm not sure what the casual user would use this banner class for, but here it is.
--->
{{banner
A companion to the fifth Edition [*Dungeon's Masterguide*](https://homebrewery.naturalcrit.com/share/2468EmsFzBJR){color:white} <br> (2024) and [*Monster's Manual*](https://homebrewery.naturalcrit.com/share/0ald8nfxDSTm){color:white} (2025)
}}

<!---
The logo portion emulates the gold foil on the backs of the new books. The words are dynamic and will show the gold texture behind it, but the image is static and is made to look like gold; other images won't look gold like this automatically. 

This means that you can use whatever image you like for the logo bit! I recommend using the Homebrewery logo anyways; it looks nice, and the HB is coming up on its 10th anniversary next year!
--->
{{logo
![HB 10th Anniversary!](https://ik.imagekit.io/kaiburrkathhound/10thAnniversary.webp)

10th Anniversary
___

[Homebrewery.Naturalcrit.com](https://www.naturalcrit.com/)
}}

}}

