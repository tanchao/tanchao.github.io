require "fileutils"

desc "create new posts"
task :newdoc do
    puts "enter new post url: "
    @url = STDIN.gets.chomp
    puts "enter title: "
    @title = STDIN.gets.chomp
    puts "enter sub-title: "
    @subtitle = STDIN.gets.chomp
    puts "enter categories (split by <space>): "
    @cates = STDIN.gets.chomp
    puts "enter tags: "
    @tags = STDIN.gets.chomp
    
    @slug = "#{@url}"
    @slug = @slug.downcase.strip.gsub(" ", "-")
    @date = Time.now.strftime("%F")
    @post_name = "_posts/#{@date}-#{@slug}.md"
    if File.exist?(@post_name)
        abort("file already exsits, aborted.")
    end
    FileUtils.touch(@post_name)
    open(@post_name, "a") do |file|
        file.puts "---"
        file.puts "layout: post"
        file.puts "title: #{@title}"
        file.puts "subtitle: #{@subtitle}"
        file.puts "author: tanchao"
        file.puts "date: #{Time.now}"
        file.puts "categories: #{@cates}"
        file.puts "tags: #{@tags}"
        file.puts "---"
    end
    exec "vim #{@post_name}"
end
