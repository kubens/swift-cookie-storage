# swift-cookie-storage

A cross-platform Swift Package Manager library providing RFC6265-compliant HTTP cookie management for Apple platforms, Linux, and Swift on Server frameworks.

[![Swift 6.0+](https://img.shields.io/badge/Swift-6.0+-orange.svg)](https://swift.org)
[![Platforms](https://img.shields.io/badge/Platforms-macOS%20|%20iOS%20|%20watchOS%20|%20tvOS%20|%20Linux-lightgrey.svg)](https://swift.org)
[![SPM Compatible](https://img.shields.io/badge/SwiftPM-Compatible-brightgreen.svg)](https://swift.org/package-manager)

## Features

- 🎯 **RFC6265 Compliant**: Full implementation of HTTP State Management Mechanism specification
- 🌍 **Cross-Platform**: Pure Swift implementation supporting Apple platforms and Linux
- ⚡ **High Performance**: UTF-8 level parsing with optimized cookie operations
- 🔒 **Thread Safe**: Actor-based concurrency model for safe concurrent access
- 🖥️ **Server Ready**: Designed for Swift on Server frameworks (Vapor, Hummingbird)
- 📊 **Comprehensive**: All standard cookie attributes with proper validation

## RFC6265 Compliance

This library implements the full RFC6265 specification including:

### Cookie Parsing (Section 4.1)
- ✅ Cookie name/value extraction with proper token validation
- ✅ Case-insensitive attribute parsing  
- ✅ Whitespace handling and trimming
- ✅ Malformed input rejection

### Domain Matching (Section 5.2.3)
- ✅ Exact domain matching
- ✅ Subdomain matching with proper dot handling
- ✅ Leading dot normalization
- ✅ Public suffix protection

### Path Matching (Section 5.2.4)  
- ✅ Path prefix matching
- ✅ Default path handling
- ✅ Case-sensitive path comparison

### Attribute Handling
- ✅ **Expires**: RFC-compliant date parsing (multiple formats)
- ✅ **Max-Age**: Takes precedence over Expires
- ✅ **Secure**: HTTPS-only cookie transmission
- ✅ **HttpOnly**: Script access prevention
- ✅ **SameSite**: CSRF protection

### Cookie Ordering (Section 5.4)
- ✅ Longer paths first
- ✅ Creation time ordering for equal paths

## Requirements

- **Swift**: 6.0 or later
- **Platforms**: 
  - macOS 10.15+
  - iOS 13.0+
  - watchOS 6.0+  
  - tvOS 13.0+
  - Linux (Swift 6.0+)

## Testing

Run the comprehensive test suite:

```bash
swift test
```

The library includes extensive RFC6265 compliance tests covering edge cases, malformed input, and cross-platform behavior.

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow Swift API Design Guidelines
- Maintain RFC6265 compliance
- Add tests for new functionality
- Update documentation for public APIs
- Ensure cross-platform compatibility

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
