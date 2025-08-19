# ChessGame
C# WPF chess game (ChessUI + ChessLogic) built for SWE40006. Packaged with WiX (MSI) and an optional MSIX sideload bundle. Download installers from Releases.

#One-paragraph intro (README top)

Chess Game (C# · WPF · .NET 6) — a simple, student-built chess app created for the SWE40006 Software Deployment & Evolution unit. The UI (ChessUI) handles the board and moves, and a small library (ChessLogic) validates basic rules. The project focuses on Windows deployment: a WiX MSI that installs to Program Files and creates a Start menu shortcut, plus an MSIX sideload package for modern packaging. Grab the installer from Releases, or build from source with Visual Studio 2022.

🧭# Longer description (README section)

This repository contains a WPF chess game packaged two ways to demonstrate Windows deployment:

ChessUI (WPF, .NET 6) – user interface, board rendering, basic interactions

ChessLogic (Class Library) – move validation and simple rule checks

SetupProject1 – WiX Toolset project that produces an MSI (installs to C:\Program Files\Chess Game and adds a Start menu shortcut)

ChessApp – Windows Application Packaging Project that produces an MSIX sideload bundle

The goal is to document a clean deployment pipeline for a small desktop app, including handling DLL dependencies, passing WiX ICE validation (separate component for the shortcut with an HKCU KeyPath), and fixing common issues like architecture mismatches and RID restores.

Downloads: see Releases for the MSI (recommended for marking) and an optional MSIX test bundle.
Install: run the MSI; for MSIX, run Add-AppDevPackage.ps1 (Admin) to trust the test certificate and install.
Built with: C#, .NET 6, WPF, WiX Toolset 3.11/3.14, Windows Application Packaging Project, Visual Studio 2022.
Course context: developed as part of the OOP/Deployment portfolio (SWE40006).

📥# Quick install (to include in README)
1) Download the latest MSI from Releases and run it.
2) Start Menu → Chess.
(Optional) MSIX: download the MSIX bundle, right-click Add-AppDevPackage.ps1 → Run with PowerShell (Admin).

🏷 #Suggested topics/tags

csharp dotnet wpf wix msi msix windows-installer desktop-app chess student-project
