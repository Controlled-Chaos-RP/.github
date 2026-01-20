# Hightower Framework (HT-Framework)

**Developer:** Hightower Scripts  
**Exclusive for:** Controlled Chaos Roleplay Server

---

## 🎮 About

The **HT-Framework** is a custom-built, modular FiveM roleplay framework created exclusively for the **Controlled Chaos Roleplay** community. Built from the ground up with security, performance, and flexibility in mind, this framework provides a comprehensive foundation for immersive roleplay experiences.

### 🔗 Community Links

- **Discord:** [https://discord.controlledchaos.life](https://discord.controlledchaos.life)
- **Website:** [https://www.controlledchaos.life](https://www.controlledchaos.life)

---

## 📦 Framework Modules

### Core Systems

#### **ht-core**
The foundation of the framework providing player session management, multi-character support (up to 3 characters per account), secure authentication, RPC communication layer, database wrapper, and modern NUI interface. Essential dependency for all other modules.

#### **ht-multichar**
Multi-character management system with character creation, selection, and deletion. Features secure validation, ownership verification, and elegant UI integration.

---

### Economic Systems

#### **ht-bank**
Comprehensive banking and currency management system handling bank accounts, cash transactions, ATM interactions, and secure player-to-player money transfers with anti-exploit protection.

#### **ht-payroll**
Automated payroll processing system with multi-job support, configurable tax rates, employer deductions, persistent paycheck history, and automatic bank integration.

---

### Player Systems

#### **ht-apartments**
Apartment and spawn management system featuring starter motels for new players, purchasable apartments with IPL interiors, multiple spawn options, and automatic refund system (50% on sale).

#### **ht-phones**
Feature-rich phone system with mobile phones (smartphones and burner phones), calling functionality, text messaging, contact management, call history, payphone locations, and pma-voice integration.

#### **ht-jobs**
Multi-job management system allowing players to hold multiple jobs simultaneously with duty status tracking, grade systems, salary management, and public job center access.

---

### Gameplay Systems

#### **ht_garbagejob**
Zone-based garbage collection job with free-roam gameplay, multiple depot locations (Alta Street, Sandy Shores, Paleto Bay), vehicle rentals, real-time HUD tracking, and comprehensive anti-exploit protection.

---

## 🏗️ Architecture

The framework follows a modular design pattern where `ht-core` serves as the central dependency, providing essential services to all other modules including:

- Player and character management
- Database operations via oxmysql
- RPC (Remote Procedure Call) system for secure client-server communication
- Event handling and state management
- NUI interface framework

All modules are designed with:

- ⚡ **Performance optimization** - Minimal resource impact
- 🛡️ **Security hardening** - Input validation, rate limiting, exploit prevention
- 🔄 **Server-authoritative logic** - Critical operations validated server-side
- 📝 **Comprehensive logging** - Audit trails for important actions

---

## 🔧 Dependencies

The framework requires the following external dependencies:

- **oxmysql** - MySQL database wrapper
- **ox_lib** - UI library for context menus and notifications
- **pma-voice** - Voice system for phone call functionality (recommended)

---

## 📋 Installation

1. Ensure all dependencies are installed and configured
2. Place the `[ht-framework]` folder in your FiveM server's `resources` directory
3. Add the following to your `server.cfg` in order:
   ```
   ensure ht-core
   ensure ht-multichar
   ensure ht-apartments
   ensure ht-bank
   ensure ht-payroll
   ensure ht-phones
   ensure ht-jobs
   ensure ht_garbagejob
   ```
4. Configure each module's settings in their respective `config` or `shared/config.lua` files
5. Restart your server

---

## 📄 License

All modules in this framework are licensed and exclusive to **Controlled Chaos Roleplay**. Unauthorized distribution or use is prohibited.

---

## 🔒 Security

Security is a top priority across all modules. Each resource implements:
- Server-side validation for all critical operations
- Rate limiting to prevent abuse
- Input sanitization and type checking
- Authorization verification
- Transaction locks for database operations
- Comprehensive audit logging

For detailed security information on individual modules, see their respective `docs/VERSIONS.md` files.

---

## 📞 Support

For support, questions, or to join our community:
- Join our Discord: [https://discord.controlledchaos.life](https://discord.controlledchaos.life)
- Visit our website: [https://www.controlledchaos.life](https://www.controlledchaos.life)

---

**© 2026 Hightower Scripts | Controlled Chaos Roleplay**
