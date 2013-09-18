#!/usr/bin/env ruby

desc "Generate a new post"
task :post, [:slug] do |t, args|
  stamp = Time.now.strftime("%Y-%m-%d")
  time = Time.now.strftime("%H:%M")
  f = File.open("_posts/#{stamp}-#{args.slug}.md", "w").write(<<eos)
---
title: #{args.slug}
layout: post
date: #{stamp} #{time}
---


eos
end
