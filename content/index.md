+++
Title = "Home"
+++

# Nice To Know

This is a collection of mind maps of stuff that is nice to know.

## …about what?

Everything! We started with IT, because we're IT-guys, but you can create any repo you know things about!

See the list of repositories here: https://github.com/NiceToKnow

## GitHub + Folders = Collaborative Mind Map

Mind maps should be easy. Collaborative mind maps usually are not, because the underlying structure is unclear and the tools for versioning are bad. But why not use already existing tools that are great?

    underlying structure => folders and files
    versioning => git

To connect those two, we use a little helper called [Hugo](http://gohugo.io/). It creates web-pages from folders and markdown files.

## Is there a preferred structure?

Yes, there is, and it is needed for Hugo to create the proper connections:

    root
    ├── content (the source files)
    │   ├── Topic A
    │   │    ├── Topic A.md (a description of that topic)
    │   │    └── Subtopic 1
    │   │        ├── Subtopic 1.md (a description of the subtopic)
    │   │        ├── Sub-Subtopic X.md (a description of the sub-subtopic)
    │   │        ├── Sub-Subtopic Y.md (a description of the sub-subtopic)
    │   │        └── Sub-Subtopic Z.md (a description of the sub-subtopic)
    │   ├── Topic B 
    │   │    └── ...
    ├── public (the generated files)
    ├── themes
    │   ├── folderMap (the basis for html output)
    ├── deploy.sh (to make your life easier)
    └── ...

You will only work in the `content` folder, and that structure should be very easy (otherwise simplify it!) :)