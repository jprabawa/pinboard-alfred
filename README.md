# Pinboard for Alfred

This is a very simple ruby script to add a URL with a title to Pinboard.
The script makes use of the [Pinboard API](http://pinboard.in/api).

## Installation

The script requires the [escape gem](http://rubygems.org/gems/escape) to be installed. The Gemfile is included so you just need to run [bundler](http://gembundler.com):

<pre>bundle install</pre>

## Usage

Add a new URL from http://url with the title *"Multiword Title"*:
<pre>pinboard http://url Multiword Title</pre>

Add a new URL from http://url with the title *"http://url"*:

<pre>pinboard http://url</pre>

## Creating The Alfred Extension

You can follow the lovely instructions by Andrew Pepperrell [here](http://preppeller.com/2011/12/11/creating-an-alfred-extension-101/).

In the command text area, you use:
<pre>/path/to/pinboard #{query}</pre> 

If you enable Notification Center, the script will output the Pinboard API status code on completion, e.g. "done" when the URL was added successfully.

## License

Standard [MIT License](http://opensource.org/licenses/MIT)