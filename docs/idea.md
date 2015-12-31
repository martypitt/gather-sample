# Gather Wiki

A wiki-like thing that pulls static content from git repos.

 * I create a project
 * I add multiple git repo's to the project
 * The projects are cloned.  The content of /docs is parsed, and injested as content
 * Content is indexed & searchable
 * Content that is on `master` is considered current
 * Content that is on branches are considered proposed
    * Content that is proposed, but hasn't been modified or merged in some time becomes 'stale'
 * As updates are merged, history is archived.

## Benefits
 * Content evolves with the code -- requirements describe either current, or intended system state
 * Allow image capture of 'expected' state of HTML components -- better integration with CI servers
 
## Collaboration
 * Content can be discussed -- comments are held on the app, and are considered non canonical
 * Proposals (branches) can be discussed in-line.  Comments are not merged, as they are non canonical.
 * `master` cannot be discussed, but can show active proposals (and associated discussions)
 * `master` allows creating a proposal (ie., branching, and editing a file)

## Rendering
 * Allow a pluggable renderer model.
    * `*.txt`, Markdown, HTML, `*.feature?`, images

## Plugin ideas
 * Show me which features are currently passing (Build server integration)
 * in-place editor(s) -- different per content?
 
 