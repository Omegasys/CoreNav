==================================================
CORENAV CLI SPECIFICATION
Version 1.0 Draft

PURPOSE

The Command Line Interface provides direct scripting,
automation, remote administration, and advanced user
interaction with CoreNav.

Every CoreNav operation shall be available through
CLI commands.

==================================================
DESIGN GOALS

Scriptable

Automatable

Remote Friendly

Machine Readable

Human Readable

Feature Complete

==================================================
COMMAND STRUCTURE

corenav   [options]

Examples

corenav file copy
corenav file move
corenav project build
corenav project run
corenav plugin install
corenav terminal open

==================================================
FILESYSTEM COMMANDS

corenav file list

corenav file copy

corenav file move

corenav file rename

corenav file delete

corenav file secure-delete

corenav file search

corenav file tag

corenav file hash

corenav file permissions

==================================================
DIRECTORY COMMANDS

corenav dir create

corenav dir remove

corenav dir organize

corenav dir sync

corenav dir size

==================================================
ARCHIVE COMMANDS

corenav archive create

corenav archive extract

corenav archive verify

corenav archive browse

==================================================
PROJECT COMMANDS

corenav project list

corenav project open

corenav project build

corenav project run

corenav project test

corenav project clean

corenav project dependencies

==================================================
WORKSPACE COMMANDS

corenav workspace create

corenav workspace load

corenav workspace save

corenav workspace list

corenav workspace delete

==================================================
TERMINAL COMMANDS

corenav terminal open

corenav terminal close

corenav terminal list

corenav terminal profile

corenav terminal sync

corenav terminal execute

==================================================
PLUGIN COMMANDS

corenav plugin list

corenav plugin install

corenav plugin remove

corenav plugin update

corenav plugin enable

corenav plugin disable

corenav plugin permissions

==================================================
SECURITY COMMANDS

corenav security hash

corenav security sign

corenav security verify

corenav security trust

corenav security sandbox

==================================================
DEVICE COMMANDS

corenav device list

corenav device inspect

corenav device monitor

==================================================
NETWORK COMMANDS

corenav network ssh

corenav network sftp

corenav network mount

corenav network browse

==================================================
GIT COMMANDS

corenav git status

corenav git log

corenav git branch

corenav git diff

corenav git commit

corenav git merge

==================================================
SYSTEM COMMANDS

corenav system status

corenav system processes

corenav system services

corenav system resources

==================================================
OUTPUT MODES

Human

JSON

YAML

XML

CSV

Markdown

==================================================
AUTOMATION

Shell Scripting

Cron Jobs

Systemd Services

CI/CD Integration

Plugin Automation

==================================================
PRIVILEGE MANAGEMENT

Commands requiring elevated privileges shall request:

* Password
* FIDO2
* Security Key
* Smart Card
* Biometrics
* Policy Authorization

No command shall silently elevate privileges.

==================================================
COMMAND DISCOVERY

corenav help

corenav help 

corenav search-command

corenav command-palette

==================================================
INTERFACE PARITY

All GUI Features

All TUI Features

All Plugin Features

All Workspace Features

shall be accessible from the CLI.

==================================================
END SPECIFICATION