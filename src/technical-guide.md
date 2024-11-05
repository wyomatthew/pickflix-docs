# Technical Guide

This documents provides a technical description of how Pickflix operates. All of
the source for Pickflix is open to view on GitHub at
[wyomatthew/pickflix](https://github.com/wyomatthew/pickflix).

## Service Architecture

Below is a diagram describing the architecture and software stack of Pickflix:

<img src="images/diagram.svg" alt="Pickflix Architecture Diagram" stroke="none" fill="none"/>

## Deployment Environment

All self-hosted services (ie all applications within the "PICKFLIX" box in the
[service architecture](#service-architecture)) are hosted as Docker containers
on a custom-built home server. The server contains **26TB** of storage for
storing media ready to be streamed.
