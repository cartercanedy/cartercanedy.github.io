+++
title = "About me"
date = "2024-12-25"
aliases = ["about-me", "contact"]
[author]
name = "Carter Canedy"
+++

In my day job, I'm a scientist and software engineer for Novartis BioMedical Research.
I've helped to engineer the cutting edge of complex cellular modelling, designed and implemented
a scientific data management and processing platform, and more.

In my own time, I'm busy being a FOSS advocate. I've started a few projects of my own, and
I'm helping out with others. I've been using Rust for my last few projects, but I'm a polyglot
by necessity. I've worked extensively with Python, JavaScript, TypeScript, React, C#, C++,
C, and mutliple PLC heuristics, so you could say that I'm well traveled in software development.

At home, I'm blessed to have a beautiful family at my side supporting me. God gave my wife and I
the blessing of two beautiful daughters who rule our worlds. Being a parent is hard, but we're
committed to being the best parents we could possibly be for them.

<br/>

---

<style>
._content {
    display: flex;
    flex-direction: column;
    justify-items: left;
    padding-top: 0rem;
    padding-bottom: 0rem;
}

._content-item {
    display: flex;
    flex-direction: column;
    justify-content: left;
    margin-top: 0;
    margin-bottom: 0;
    width: 100%;
}

.project-details-heading {
    display: inline-flex;
    font-size: 1.5rem;
    align: center;
}

.project-details-subheading {
    display: block;
    font-size: 1.125rem;
}

.project-details-content {
    display: block;
    font-size: 1rem;
}

</style>

<link rel="stylesheet" href="../css/util.css"/>

<h2 class="my-0" style="margin-top: 2rem">Projects</h2>

<br/>
<div class="_content">
    <div class="_content-item">
        <p class="m-0 project-details-heading"><a href="https://github.com/cartercanedy/rawbit">rawbit</a></p>
        <p class="my-1 project-details-subheading">A batch camera RAW image preprocessor and DNG converter</p>
        <p class="my-1 project-details-subheading">Technologies: Rust</p>
        <p class="m-2 project-details-content">
            This was a personal project driven by my need to reduce my dependence on the Adobe image processing software suite.
            I initially began implementing this project with Python, but I was immediately put off by a combination of performance
            issues and high-level RAW image manipulation library support (or lack thereof).
            <br/><br/>
            I had already worked with Rust at my day job prior to becoming a Rust contributor to the
            <a href="https://github.com/christitustech/linutil">linutil</a>
            project, so I decided to investigate the feasibility of a Rust-based implementation. After some bit of digging, I
            found the
            <a href="https://github.com/dnglab/dnglab/blob/refs/master/rawler">rawler</a>
            project, written from the ground up in Rust for high-level RAW image conversion to the DNG format. As for
            performance, I found that it's pretty-much brain-dead easy to implement basic parallelization via the
            <a href="https://github.com/rayon-rs/rayon">rayon</a>
            library.
            <br/><br/>
            Since the single-file prototype, I've made some pretty substantial rewrites to make better use of CPU time with async using
            <a href="https://github.com/tokio-rs/tokio">tokio</a>,
            and I've spent a lot of time to ensure that I have a comprehensive CI/CD/testing workflows to make maintenance simple
            moving forward.
        </p>
    </div>
    <br/>
    <div class="_content-item">
        <p class="m-0 project-details-heading"><a href="https://github.com/christitustech/linutil">linutil</a></p>
        <p class="my-1 project-details-subheading">A TUI designed to speed up common setup tasks on any Linux distro</p>
        <p class="my-1 project-details-subheading">Technologies: Rust, Shell scripting</p>
        <p class="m-2 project-details-content">
            The linutil project provides a bunch of pre-written shell scripts to perform common tasks on Linux systems. It doesn't require
            any shell scripting knowledge, and can install new software, provides reasonable defaults for software configurations, and
            perform common system maintenance tasks, all bundled into an easy-to-use terminal user interface.
        </p>
    </div>
    <br/>
    <div class="_content-item">
        <p style="text-decoration: underline" class="m-0 project-details-heading">OctoPi</p>
        <p class="my-1 project-details-subheading">A prototype instrument for capturing contractility data from 3D cardiomyocyte cultures</p>
        <p class="my-1 project-details-subheading">Technologies: Python, Rust, Beckhoff PLC, distributed embedded computation</p>
        <p class="m-2 project-details-content">
            The OctoPi is a first-of-its-kind instrument enabling high-throughput research working with iPSC-derived cardiomyocyte cultures.
            Scientists are able to use standard 96- or 384-well microplates to culture cardiomyocyte organoids in 3D and assess the affects of
            any kind of perturbant on contractility, enabling large-scale experiments that weren't possible using other commercial solutions.
        </p>
    </div>
    <br/>
    <div class="_content-item">
        <p class="m-0 project-details-heading"><a href="https://github.com/cartercanedy/zips">zips</a></p>
        <p class="my-1 project-details-subheading">A simple Rust macro for performing <code>Option::zip</code> over an arbitrary number of <code>Option</code>s or <code>Result</code>s</p>
        <p class="my-1 project-details-subheading">Technologies: Rust</p>
        <p class="m-2 project-details-content">
            This one was born out of a need to ergonomically zip up a bunch of fallible operations together.
            <br/><br/>
            It's not always the most useful, but you won't need it until you do, and I did.
        </p>
    </div>
    <br/>
</div>
