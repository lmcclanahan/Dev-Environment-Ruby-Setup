# Dev-Environment-Ruby-Setup
ruby devkit, gems, nuget, chocolatey rake

downloads and installs Chocolatey
installs nuget.commandline if it is not installed
installs ruby.devkit if it is not installed
installs ruby if it is not installed
updates gems and installs some required gems for rake
restores nuget packages from the configs
builds the source with rake

@echo off
SET DIR=%~dp0%
@PowerShell -NoProfile -ExecutionPolicy unrestricted -Command "& '%DIR%setup.ps1' %*"
pause
