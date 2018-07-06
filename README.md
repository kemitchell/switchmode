![Switchmode](./switchmode.png)

# Switchmode Developer Agreement

an open form contract for open source contractors

Download the most recent release from [GitHub](https://github.com/switchmode/switchmode/releases) or [commonform.org](https://commonform.org/switchmode).

## Be Warned!

**Contracts are prescription-strength legal devices.  If you need terms for a contracting relationship, don't be an idiot.  Hire a lawyer.  A good one will ask good questions. They may decide this form fits your needs.**

**Do _not_ put confidential information about you, your work, or your clients in issues or pull requests.  Do _not_ ask for legal advice on GitHub, or try to disguise requests for legal advice as general questions or hypotheticals.  You don't want advice from anybody dumb enough to fall for that.**

## In Brief

The Switchmode Developer Agreement is a new breed of independent contractor agreement for open-source developers doing a mix of open and closed projects for clients.  Unlike a "traditional", Silicon Valley-style independent contractor or consulting agreement, Switchmode addresses the use and release of open-source software directly.

### New and Novel

Switchmode uses the terms of an open-source license, The Apache License, Version 2.0, as the terms of license between developer and client.  Most clients' lawyers know Apache well, and use a ton of software under its terms already.  To address additional, reasonable expectations for paid work, Switchmode layers additional terms about provenance and ownership on top of Apache for work from the developer.

Switchmode sets up an open release process the developer can use to request permission to publish reusable components of company-owned, closed-project work under The Apache License.  When approved, the developer can release code under an Apache License under sublicense through Switchmode, without disclosing who the client was.  The client can optionally choose direct attribution.

Plain-language, two-way confidentiality terms cover all projects and work.  There's an explicit exception for approved open releases, as well as a special exception for disclosing technical details when working with developers of open-source software used for a project.

Both the open release process and community-work exception involve a "technical representative" who speaks for the client on engineering matters with low legal and business risk.

### Structure

Switchmode is structured as a master agreement setting out terms that apply to work agreed in "Project Summaries" signed by developer and client.  There are all kinds of names for this kind of arrangement: statements of work, work orders, and so on.

Each Project Summary describes the work to be done on a project, what the client will pay for it, and whether it is an "open project" or a "closed project".  Different intellectual property and confidentiality terms apply to work on the project, depending on whether it's closed or open.

Switchmode comes with a number of starting-point templates for projects of various kinds.

## Building

The repository has configuration to build copies of the terms in various formats, including Word, PDF, Markdown, and native Common Form.

If you're alright agreeing to the terms of use for Microsoft's Core Fonts for the Web, for Times New Roman, the easiest way to build is probably with Docker:

```shellsession
git clone https://github.com/switchmode/switchmode
cd switchmode
git checkout $edition
make docker
```

The `Dockerfile` uses a Debian Linux base image for Node.js, and installs other build tools from Debian package repositories.  If you want to build without Docker, have a look at the `RUN` lines in `Dockerfile` to see what you'll need.

## Thanks

The Switchmode Developer Agreement can only improve and succeed with the help of community members---lawyers, coders, and businessfolk---who take time to share their thoughts and experiences.  In addition to the Git commit log, see [`THANKS.md`](THANKS.md) for thanks and credits.
