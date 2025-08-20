## Installing Marzban

### 🔧 Available options

| Option               | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `--database`         | Optional. Choose from: `mysql`, `mariadb`, `postgres`, `timescaledb`. Default is `sqlite`. |
| `--version <vX.Y.Z>` | Install a specific version, including pre-releases (e.g., `v0.5.2`, `v1.0.0-beta.1`)                               |
| `--dev`              | Install the latest development version (only for versions **before v1.0.0**) |
| `--pre-release`      | Install the latest pre-release version (only for versions **v1.0.0 and later**) |

> ℹ️ `postgres` and `timescaledb` are only supported in versions **v1.0.0 and later**.  
> ℹ️ Pre-release versions (e.g., `v1.0.0-beta.1`) can also be installed using `--version`.
---

### 📦 Examples

- **Install Marzban with SQLite**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install
  ```

- **Install Marzban with MySQL**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install --database mysql
  ```
- **Install Marzban with PostgreSQL(v1+ only)**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install --database postgresql
  ```
- **Install Marzban with TimescaleDB(v1+ only) and pre-release version**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install --database timescaledb --pre-release
  ```

- **Install Marzban with MariaDB and Dev branch**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install --database mariadb --dev
  ```

- **Install Marzban with MariaDB and Manual version**:

  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban.sh)" @ install --database mariadb --version v0.5.2
  ```
## Installing Gozargah-node

### 📦 Examples

- **Install Gozargah-node**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/gozargah-node.sh)" @ install
  ```
- **Install Gozargah-node Manual version:**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/gozargah-node.sh)" @ install --version 0.1.0
  ```
- **Install Gozargah-node pre-release version:**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/gozargah-node.sh)" @ install --pre-release
  ```

- **Install Gozargah-node with custom name:**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/gozargah-node.sh)" @ install --name gozargah-node2
  ```
    > 📌 **Tip:**  
    > The `--name` flag lets you install and manage multiple Gozargah-node instances using this script.  
    > For example, running with `--name gozargah-node2` will create and manage a separate instance named `gozargah-node2`.  
    > You can then control each node individually using its assigned name.

- **Update or Change Xray-core Version**:

  ```bash
  sudo gozargah-node core-update
  ```

Use `help` to view all commands:
```gozargah-node help```




## Installing Marzban-node

> ⚠️ **Deprecation Notice for Marzban-node**  
> **Important:**  
> Marzban-node has been deprecated and is no longer actively maintained.

### 📦 Examples

- **Install Marzban-node**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban-node.sh)" @ install
  ```
- **Install Marzban-node with custom name:**
  ```bash
  sudo bash -c "$(curl -sL https://github.com/RZAsadi/Marzban-scripts/raw/master/marzban-node.sh)" @ install --name marzban-node2
  ```
    > 📌 **Tip:**  
    > The `--name` flag lets you install and manage multiple Marzban-node instances using this script.  
    > For example, running with `--name marzban-node2` will create and manage a separate instance named `marzban-node2`.  
    > You can then control each node individually using its assigned name.

- **Update or Change Xray-core Version**:

  ```bash
  sudo marzban-node core-update
  ```

Use `help` to view all commands:
```marzban-node help```
