---
layout: post
title: "Sesar lembang yang tertunda"
description: ""
date: 2020-10-31
categories: ''
inreview: true
tags: []
permalink: /sesarlembang2020
comments: true
share: true
hidden: true
---

<style>
$primary: #fc5a7d
$secondary: #7d6dfb
$dark: #18294f
$timeline-1: #fec541
$timeline-2: #36d484
$timeline-3: #32ccf4
$timeline-4: #fd9252
$bg-mild: #f5f7f6
$bg-reg: #dfe3e6
$bg-dark: #7f9298
$text-black: #4A4A4A

body
  // background-color: $bg-mild
  margin: 0

.body-wrap
  background-color: #fff
  width: 600px
  min-height: 500px
  margin: 0 auto
  font-size: 12px
  
.pres-timeline
  font-family: roboto, helvetica, sans-serif
  font-size: 12px
  color: $text-black
  width: 100%
  margin: 30px 0
  > div > div a
    // this is  fixing the padding bug
    padding: 1em 0
    box-sizing: border-box
  
  .periods-container, .cards-container
    overflow: hidden
    box-sizing: border-box
    position: relative
    min-height: 100px
    transition: height .5s ease-in-out
    background-color: #FFF
  .timeline-container
    
.periods-container
  &:before
    background-image: linear-gradient(left, #FFF, rgba(248, 248, 248, 0))
    left: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  &:after
    background-image: linear-gradient(right, #FFF, rgba(248, 248, 248, 0))
    right: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  .btn-back, .btn-next
    // background-color: 
    // border: 2px solid $bg-reg
    display: inline-block
    width: 15%
    height: 100%
    position: absolute
    cursor: pointer
    z-index: 10
    transition: 0.3s ease-in-out
    &:hover
      background-color: rgba(0,0,0,.05)
    &.hide
      display: none
  .btn-back
    left: 0
  .btn-next
    right: 0
  section
    width: 70%
    height: 0
    position: absolute
    margin-left: 15%
    // border: 1px solid $bg-mild
    border-bottom: 5px solid $bg-reg
    padding: 1.5em
    box-sizing: border-box
    transition: transform .3s ease-in-out, opacity .2s ease, height .3s ease
    bottom: 0
    opacity: 0
    background-color: #fff
    &.active
      height: auto
      opacity: 1
      transform: translateX(0)
      z-index: 5
      .title, p
        display: block
    &.prev
      height: auto
      opacity: 0.4
      transform: translateX(-100%)
      z-index: 0
      .year
        text-align: right
    &.next
      height: auto
      opacity: 0.4
      transform: translateX(100%)
      z-index: 0
    .year
      font-size: 20px
      font-weight: 400
    .title
      color: $text-black
      font-size: 28px
      font-weight: 400
      display: none
    p
      display: none
// Timeline styles
.timeline-container
  position: relative
  width: 100%
  height: 50px
  overflow: hidden
  &:before
    background-image: linear-gradient(left, #FFF, rgba(248, 248, 248, 0))
    left: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  &:after
    background-image: linear-gradient(right, #FFF, rgba(248, 248, 248, 0))
    right: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  .timeline
    position: absolute
    display: block
    height: 50px
    transition: left .3s ease-in-out
    ol
      display: block
      width: 100%
      height: 2px
      background-color: $bg-reg
      list-style: none
      padding-left: 210px
      padding-right: 300px
      li
        display: inline-block
        padding: 5px
        margin-top: -11px
        margin-left: 80px
        border-radius: 50%
        border: 3px solid $bg-dark
        background-color: #FFF
        position: relative
        cursor: pointer
        box-shadow: 0 2px 5px rgba(0,0,0,.2)
        &.active
          box-shadow: none
        &.active:before
          content: ""
          display: block
          height: 25px
          width: 1px
          position: absolute
          top: -25px
          transition: opacity .3s ease-in-out
          // opacity: 0
        &.active:after
          content: ""
          display: block
          height: 25px
          width: 1px
          position: absolute
          bottom: -25px
          transition: opacity .3s ease-in-out
          // opacity: 0
  .btn-back, .btn-next
    display: inline-block
    position: absolute
    cursor: pointer
    margin-top: -2px
    z-index: 11
    transition: all .3s ease
    &.hide
      display: none
      
    &:hover
      border-color: $bg-dark
  .btn-back
    left: 1em
    // background: url('data:image/svg+xml;utf8,<svg width="14" height="22" viewBox="6 4 14 22" xmlns="http://www.w3.org/2000/svg"><path fill="#D8D8D8" fill-rule="evenodd" d="M11.828 15l7.89-7.89-2.83-2.828L6.283 14.89l.11.11-.11.11L16.89 25.72l2.828-2.83"/></svg>') no-repeat
  .btn-next
    right: 1em
    // background: url('data:image/svg+xml;utf8,<svg width="14" height="23" viewBox="10 3 14 23" xmlns="http://www.w3.org/2000/svg"><path fill="#D8D8D8" fill-rule="evenodd" d="M18.172 14.718l-7.89-7.89L13.112 4l10.606 10.607-.11.11.11.11-10.608 10.61-2.828-2.83 7.89-7.89"/></svg>') no-repeat
    
// Cards
.cards-container
  // &:after
  //   content: ""
  //   display: block
  //   width: 100%
  //   height: 2em
  //   background-image: linear-gradient(bottom, #FFF, rgba(248, 248, 248, 0))
  //   position: absolute
  //   bottom: 0
  &:before
    background-image: linear-gradient(left, #FFF, rgba(248, 248, 248, 0))
    left: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  &:after
    background-image: linear-gradient(right, #FFF, rgba(248, 248, 248, 0))
    right: 0
    content: ''
    position: absolute
    z-index: 2
    top: 0
    height: 100%
    width: 100px
  section
    width: 70%
    position: absolute
    margin-left: 15%
    margin-bottom: 2em
    border: 1px solid $bg-mild
    padding: 1.5em
    box-sizing: border-box
    transition: transform .3s ease-in-out
    top: 0
    opacity: 0
    border-radius: 8px
    background-color: #fff
    box-shadow: 0 10px 15px rgba(0,0,0,.15)
    &.active
      height: auto
      opacity: 1
      transform: translateX(0)
      z-index: 5
    &.prev
      height: auto
      opacity: 0.4
      transform: translateX(-105%)
      z-index: 0
    &.next
      height: auto
      opacity: 0.4
      transform: translateX(105%)
      z-index: 0
    .year
      text-align: center
      font-size: 16px
      margin: 0
    .title
      font-weight: 400
    img
      width: 100%
</style>

<script>
    class PRESTimeline {
  
  base: HTMLElement
  periodContainer: HTMLElement
  cardContainer: HTMLElement
  activePeriod: HTMLElement
  activeCard: HTMLElement
  activePeriodIndex: number
  activeCardIndex: number
  periodData: object[]
  cardData: object[]
  color: object
  timelineNodeContainer: HTMLElement
  timelineData: object[]
  
  constructor(target: HTMLElement, color: object){
    
    // this.__process_stylesheet(document.styleSheets[0]);
    
    this.base = target
    this.color = color
    // console.log(this.color)
    this.periodContainer = $(this.base).find('.periods-container')
    this.cardContainer = $(this.base).find('.cards-container')
    this.timelineNodeContainer = $(this.base).find('.timeline-container .timeline')
    // this.activePeriod = $(this.base).find('.periods-container section.active')
    this._parseData()
    this._initialColor()
    this._generateTimeline()
    this._setStateClasses()
    this._assignBtn()
    this._adjustPeriodContainer()
    this._adjustCardContainer()
    // console.log(this.cardData)
  }
  
  _parseData(){    
    let base = this.base
    let periods: object[] = $(base).find('.periods-container section')
    for (let section of periods) {
      section.period = $(section).attr('period')
      section.index = $(section).index()
    }
    // console.log(periods)
    this.periodData = periods
    let data: object[] = $(base).find('.cards-container section')
    // console.log(data)
    for(let section of data) {
      section.period = $(section).attr('period')
      section.index = $(section).index()
    }
    // console.log(data)
    this.cardData = data
    // #assign initial entry point (active items)
    this.activePeriod = this.periodData[0]
    this.activePeriodIndex = 0
    this.activeCard = this.cardData[0]
    this.activeCardIndex = 0
  }
  
  _setStateClasses(){
    // # periods
    $(this.base).find('.periods-container section.active').removeClass('active')
    $(this.base).find('.periods-container section.prev').removeClass('prev')
    $(this.base).find('.periods-container section.next').removeClass('next')
    // console.log("setclass: " + this.activePeriod.index)
    $(this.activePeriod).addClass('active')
    // console.log(this.activePeriod.index)
    // this.activePeriodIndex = this.activePeriod.index
    if ( $(this.activePeriod).prev().length != 0 ){
      $(this.activePeriod).prev().addClass('prev')
      $(this.base).find('.periods-container .btn-back').removeClass('hide')
    }else{
      $(this.base).find('.periods-container .btn-back').addClass('hide')
    }
    if ( $(this.activePeriod).next().length != 0){
      $(this.activePeriod).next().addClass('next')
      $(this.base).find('.periods-container .btn-next').removeClass('hide')
    }else{
      $(this.base).find('.periods-container .btn-next').addClass('hide')
    }
    
    // ## cards
    $(this.base).find('.cards-container section.active').removeClass('active')
    $(this.base).find('.cards-container section.prev').removeClass('prev')
    $(this.base).find('.cards-container section.next').removeClass('next')
    $(this.activeCard).addClass('active')
    // this.activeCardIndex - this.activeCard.index
    if( $(this.activeCard).prev().length != 0 ){
      $(this.activeCard).prev().addClass('prev')
    }
    if ($(this.activeCard).next().length != 0 ){
      $(this.activeCard).next().addClass('next')
    }
    
    // ## timeline 
    $(this.base).find('.timeline li.active').removeClass('active')
    // let findNode = $(this.base).find('.timeline ol li')[this.activeCard.index]
    $(this.timelineData[this.activeCard.index]).addClass('active')
    
    let timelineB = $(this.base).find('.timeline-container .btn-back')
    let timelineN = $(this.base).find('.timeline-container .btn-next')
    // console.log($(timelineN))
    if (this.activeCardIndex === 0){
      timelineB.addClass('hide')
    }else{
      timelineB.removeClass('hide')
    }
    if (this.activeCardIndex >= this.cardData.length-1) {
      timelineN.addClass('hide')
    }else{
      timelineN.removeClass('hide')
    }
  }
  // ## timeline generater
  _generateTimeline(){
    // ## create node list
    let htmlWrap = '<ol></ol>'
    $(this.timelineNodeContainer).append(htmlWrap)
    let wrap = $(this.timelineNodeContainer).find('ol')
    let numNode: number = this.cardData.length
    for (let i=0; i < numNode; i++) {
      let c = this.cardData[i].color
      let el = wrap.append('<li class="' + this.cardData[i].period + '" style="border-color: ' + c + '"></li>')
    }
    // ## width of timeline
    let nodeW: number = 200
    wrap.css('width', nodeW * numNode - 16)
    let nodeList: object[] = $(this.base).find('.timeline ol li')
    this.timelineData = nodeList
  }
  // ## assign button actions
  _assignBtn(){
    let periodPrev = $(this.base).find('.periods-container .btn-back')
    let periodNext = $(this.base).find('.periods-container .btn-next')
    periodPrev.click(()=>{
      if (this.activePeriodIndex > 0){
        // console.log('prev')
        this.activePeriodIndex -= 1
        this.activePeriod = this.periodData[this.activePeriodIndex]
        this._chainActions('period')
        this._setStateClasses()
      }
      this._adjustPeriodContainer()
    })
    periodNext.click(()=>{
      if (this.activePeriodIndex < this.periodData.length-1){
        // console.log('next' + this.activePeriodIndex)
        this.activePeriodIndex += 1
        this.activePeriod = this.periodData[this.activePeriodIndex]
        this._chainActions('period')
        this._setStateClasses()
      }
      this._adjustPeriodContainer()
  
    })
    let timelinePrev = $(this.base).find('.timeline-container .btn-back')
    let timelineNext = $(this.base).find('.timeline-container .btn-next')
    timelinePrev.click(()=>{
      if (this.activeCardIndex > 0){
        this.activeCardIndex -= 1
        this.activeCard = this.cardData[this.activeCardIndex]
        this._chainActions('timeline')
        this._setStateClasses()
      }
      this._adjustCardContainer()
      this._adjustPeriodContainer()
    })
    timelineNext.click(()=>{
      if (this.activeCardIndex < this.cardData.length-1){
        this.activeCardIndex += 1
        this.activeCard = this.cardData[this.activeCardIndex]
        this._chainActions('timeline')
        this._setStateClasses()
      }
      this._adjustCardContainer()
      this._adjustPeriodContainer()
    })
    
    // ## assign each timeline li
    for (let i = 0; i < this.timelineData.length; i++){
      $(this.timelineData[i]).click(()=>{
        this.activeCardIndex = this.cardData[i].index
        this.activeCard = this.cardData[this.activeCardIndex]
        this._chainActions('timeline')
        this._setStateClasses()
        this._adjustCardContainer()
        this._shiftTimeline()
      })
    }
  }
  // ## color ##
  _initialColor(){

    for(let i = 0; i < this.periodData.length; i++){
      let p = this.periodData[i].period
      this.periodData[i].color = this.color[p]
      let temp = this.periodData[i]
      $(temp).css('border-color', temp.color)
      $(temp).find('.year').css('color', temp.color)
      
      // ## color for timeline items, this part utilize the period name as class which will be add to the li later
      
      // ### cross browser bug fix
      let sbstyle = document.createElement("style")
      document.head.appendChild(sbstyle)
      // let sheet = document.styleSheets[0]
      sbstyle.sheet.insertRule('li.'+p+'.active { background-color: '+this.color[p]+' !important } ', 0)
      sbstyle.sheet.insertRule('li.'+p+'::before { background-color: '+this.color[p]+' } ', 0)
      sbstyle.sheet.insertRule('li.'+p+'::after { background-color: '+this.color[p]+' } ', 0)
      
    }
    for(let i = 0; i < this.cardData.length; i++){
      let p = this.cardData[i].period
      this.cardData[i].color = this.color[p]
      let temp = this.cardData[i]
      $(temp).css('border-color', temp.color)
      $(temp).find('.year').css('color', temp.color)
    }
  }
  
  _adjustPeriodContainer(){
    let activeH = $(this.activePeriod).outerHeight()
    $(this.periodContainer).height(activeH)
    console.log('top adjusted')
  }
  _adjustCardContainer(){
    let activeH = $(this.activeCard).outerHeight() + 24
    $(this.cardContainer).height(activeH)
    console.log('bot adjusted')
  }
  _shiftTimeline(){
    // #### We need to fix this part if using this component in different sizes ####
    let timelineW = $(this.base).find('.timeline-container').outerWidth()
    let timelinePadding = 210
    let timelineCenter = 300
    let liWidth = 16
    let activeNodeX = $(this.timelineData[this.activeCardIndex]).position().left
    let finalPos =   -activeNodeX + timelinePadding
    $(this.timelineNodeContainer).css('left', finalPos)
    console.log(activeNodeX)
  }
  _chainActions(state: string){
    switch (state){
      case 'period':
          console.log('period')
          if (this.activePeriod.period != this.activeCard.period){
            // ## find the closest li with the active period
            let ta: object[] = []
            for (let i = 0; i < this.cardData.length; i++){
              let temp = this.cardData[i]
              if (this.activePeriod.period === temp.period) ta.push(temp)
            }
            this.activeCard = ta[0]
            this.activeCardIndex = ta[0].index
          }

          break
      case 'timeline':
          console.log('timeline')
          if (this.activeCard.period != this.activePeriod.period){
            let ta: object
            for (let i = 0; i < this.periodData.length; i++){
              let temp = this.periodData[i]
              if (this.activeCard.period === temp.period) ta = temp
            }
            this.activePeriod = ta
            this.activePeriodIndex = ta.index
            
          }
          
          break
    }
    this._shiftTimeline()
    this._adjustCardContainer()
  }
  
  
}


// ## document load ##

$(document).ready(function(){
  let colorcode = {
    'period1':'#fec541',
    'period2':'#36d484',
    'period3':'#32ccf4'
  }
  let timeline = new PRESTimeline( $('#this-timeline'), colorcode )
})
</script>


<div class="body-wrap">
<!-- # component starts -->
  <div class="pres-timeline" id="this-timeline">
<!-- ###   -->
<!--   <div class="periods-section"> -->
    <div class="periods-container">
      <section class="period-single" period="period1">
        <h4 class="year">181x-181x</h4>
        <h2 class="title">1 Lorem ipsum dolor sit amet, consectetur adipisicing.</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium doloremque, laboriosam officia facere eligendi quam reiciendis, rem explicabo dolores tenetur libero minus, facilis quibusdam. Consectetur amet beatae fuga, architecto magnam.</p>
      </section>
      <section class="period-single" period="period2">
        <h4 class="year">182x-182x</h4>
        <h2 class="title">2 Lorem ipsum dolor sit amet, consectetur adipisicing.</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium doloremque, laboriosam officia facere eligendi quam reiciendis, rem explicabo dolores tenetur libero minus, facilis quibusdam. Consectetur amet beatae fuga, architecto magnam.</p>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium doloremque, laboriosam officia facere eligendi quam reiciendis, rem explicabo dolores tenetur libero minus, facilis quibusdam. Consectetur amet beatae fuga, architecto magnam.</p>
      </section>
      <section class="period-single" period="period3">
        <h4 class="year">183x-183x</h4>
        <h2 class="title">3 Lorem ipsum dolor sit amet, consectetur adipisicing.</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium doloremque, laboriosam officia facere eligendi quam reiciendis, rem explicabo dolores tenetur libero minus, facilis quibusdam. Consectetur amet beatae fuga, architecto magnam.</p>
      </section>
      <div class="btn-back"></div>
      <div class="btn-next"></div>
    </div>
<!--   </div> -->
<!-- ### -->
<!--   <div class="timeline-section"> -->
    <div class="timeline-container">
      <!--     # timeline graphic place holder - fill with js -->
      <div class="timeline"></div>
  
      <div class="btn-back"><svg width="30" height="30" viewBox="0 0 30 30" xmlns="http://www.w3.org/2000/svg"><path fill="none" d="M0 0h30v30H0z"/><path fill="#D8D8D8" fill-rule="evenodd" d="M11.828 15l7.89-7.89-2.83-2.828L6.283 14.89l.11.11-.11.11L16.89 25.72l2.828-2.83"/></svg></div>
      <div class="btn-next"><svg width="30" height="30" viewBox="0 0 30 30" xmlns="http://www.w3.org/2000/svg"><path fill="none" d="M0 0h30v30H0z"/><path fill="#D8D8D8" fill-rule="evenodd" d="M18.172 14.718l-7.89-7.89L13.112 4l10.606 10.607-.11.11.11.11-10.608 10.61-2.828-2.83 7.89-7.89"/></svg></div>
    </div>
<!--   </div> -->
<!-- ### -->
<!--   <div class="cards-section"> -->
    <div class="cards-container">
      <section class="card-single active" period="period1">
        <h4 class="year">1816</h4>
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <div class="content">
          <img src="https://ununsplash.imgix.net/photo-1421284621639-884f4129b61d?fit=crop&fm=jpg&h=700&q=75&w=1050" alt="" />
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore vitae sint dolore, officia esse! A recusandae nemo illum rem eos iusto repellendus, voluptatibus tempora nulla voluptatem officia inventore ea modi.</p>
        </div>
      </section>
      <section class="card-single" period="period1">
        <h4 class="year">1816</h4>
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <div class="content">
          <img src="https://ununsplash.imgix.net/photo-1421284621639-884f4129b61d?fit=crop&fm=jpg&h=700&q=75&w=1050" alt="" />
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore vitae sint dolore, officia esse! A recusandae nemo illum rem eos iusto repellendus, voluptatibus tempora nulla voluptatem officia inventore ea modi.</p>
        </div>
      </section>
      <section class="card-single" period="period2">
        <h4 class="year">1816</h4>
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <div class="content">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. A tempora blanditiis ut voluptas nisi labore quos iste totam obcaecati modi rerum iusto, voluptate odio commodi ratione amet illum dicta accusamus, ipsum ea vero neque enim, recusandae dignissimos? Quae ea aspernatur dolor atque, ipsum repellendus. Repudiandae culpa magnam, doloribus exercitationem illo impedit quasi officia, veniam vero molestiae sunt dolorem, excepturi ullam dicta sed amet provident ut soluta pariatur magni! Fugiat eveniet suscipit praesentium culpa aperiam ab nulla, exercitationem atque quod, labore, qui quaerat nihil nam laborum aliquam! Nesciunt dignissimos eaque impedit ex, architecto minima ad, temporibus rem possimus consequatur doloremque, fuga?</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore vitae sint dolore, officia esse! A recusandae nemo illum rem eos iusto repellendus, voluptatibus tempora nulla voluptatem officia inventore ea modi.</p>
        </div>
      </section>
      <section class="card-single" period="period1">
        <h4 class="year">1816</h4>
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <div class="content">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore vitae sint dolore, officia esse! A recusandae nemo illum rem eos iusto repellendus, voluptatibus tempora nulla voluptatem officia inventore ea modi.</p>
        </div>
      </section>
      <section class="card-single" period="period3">
        <h4 class="year">1816</h4>
        <h2 class="title">Lorem ipsum dolor sit amet.</h2>
        <div class="content">
          <img src="https://ununsplash.imgix.net/photo-1421284621639-884f4129b61d?fit=crop&fm=jpg&h=700&q=75&w=1050" alt="" />
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore vitae sint dolore, officia esse! A recusandae nemo illum rem eos iusto repellendus, voluptatibus tempora nulla voluptatem officia inventore ea modi.</p>
        </div>
      </section>
    </div>
<!--   </div> -->
<!-- ###   -->
  </div>
<!-- # component ends -->
</div>



# Referensi

https://codepen.io/knyttneve/pen/bgvmma
https://codepen.io/bcarvalho/pen/RZqmZX
https://uicookies.com/css-timeline/
https://codepen.io/kentchangdesign/pen/jadgvx
https://freefrontend.com/css-timelines/
