from https://gist.github.com/derickfay/74a66652b995a538e08a

# fix_presenter_note.applescript

tell application "Keynote"
	tell document 1
		set theSlides to slides
		repeat with s in the slides
			tell presenter notes of s
				set font to "arial"
				set size to 14
				set color of it to "black"
			end tell
		end repeat
	end tell
end tell
