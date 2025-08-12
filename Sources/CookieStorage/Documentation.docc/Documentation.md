# ``CookieStorage``

A cross-platform Swift Package Manager library providing RFC6265-compliant HTTP cookie management for Apple platforms, Linux, and Swift on Server frameworks.

## Overview

The `swift-cookie-storage` library offers a comprehensive, standards-compliant implementation of HTTP cookie handling as defined in RFC6265 - HTTP State Management Mechanism. Designed for cross-platform compatibility, it works seamlessly across macOS, iOS, watchOS, tvOS, Linux, and integrates with Swift on Server frameworks like Vapor and Hummingbird.

### Key Features

- **RFC6265 Compliant**: Full implementation of the HTTP State Management Mechanism specification
- **Cross-Platform**: Pure Swift implementation with no Foundation dependencies for maximum compatibility  
- **High Performance**: UTF-8 level parsing with optimized cookie lookup operations
- **Thread Safe**: Actor-based concurrency model for safe concurrent access
- **Server Framework Ready**: Designed to integrate with Vapor, Hummingbird, and other Swift on Server frameworks
- **Comprehensive Cookie Support**: All standard attributes including domain, path, expires, Max-Age, Secure, HttpOnly, and SameSite
