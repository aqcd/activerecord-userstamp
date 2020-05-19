# ActiveRecord-Userstamp [![Build Status](https://travis-ci.org/lowjoel/activerecord-userstamp.svg)](https://travis-ci.org/lowjoel/activerecord-userstamp) [![Coverage Status](https://coveralls.io/repos/lowjoel/activerecord-userstamp/badge.svg?branch=master&service=github)](https://coveralls.io/github/lowjoel/activerecord-userstamp?branch=master) [![Code Climate](https://codeclimate.com/github/lowjoel/activerecord-userstamp/badges/gpa.svg)](https://codeclimate.com/github/lowjoel/activerecord-userstamp)

## Overview

Userstamp extends `ActiveRecord::Base` to add automatic updating of `creator`, `updater`, and 
`deleter` attributes. It is based loosely on `ActiveRecord::Timestamp`.

Two class methods (`model_stamper` and `stampable`) are implemented in this gem. The `model_stamper`
method is used in models that are responsible for creating, updating, or deleting other objects.
Typically this would be the `User` model of your application. The `stampable` method is used in 
models that are subject to being created, updated, or deleted by stampers.

## Source

This is a fork of:

 - [Joel Low's](https://github.com/lowjoel) [activerecord-userstamp](https://github.com/lowjoel/activerecord-userstamp) gem
 - which is a fork of the [magiclabs-userstamp](https://github.com/magiclabs/userstamp) gem
 - which is a fork of [Michael Grosser's](https://github.com/grosser)
   [userstamp gem] (https://github.com/grosser/userstamp) 
 - which is a fork of the original [userstamp plugin](https://github.com/delynn/userstamp) by
   [delynn](https://github.com/delynn)

This gem was slightly modified to support Rails 6.0.3 which no longer allows the on: key for before_save.

## Authors
 - [DeLynn Berry](http://delynnberry.com/): The original idea for this plugin came from the Rails
   Wiki article entitled
   [Extending ActiveRecord](http://wiki.rubyonrails.com/rails/pages/ExtendingActiveRecordExample)
 - [Michael Grosser](http://pragmatig.com)
 - [John Dell](http://blog.spovich.com/)
 - [Chris Hilton](https://github.com/chrismhilton)
 - [Thomas von Deyen](https://github.com/tvdeyen)
 - [Joel Low](http://joelsplace.sg)
