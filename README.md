Takes text from standard input, tries to extract and dequote "safe link"-ified URLs, and prints the transformed result to standard output. Because obfuscating all links in e-mails and routing them through a man in the middle--which I'm just supposed to trust will endure for all time--is not actually a form of safety.

I am using this in conjunction with the [urlview](https://packages.debian.org/sid/misc/urlview) tool. My mutt configuration has

    macro index,pager "\Cb" "<pipe-message>antioutlook | urlview<enter>"

It requires python 3.
