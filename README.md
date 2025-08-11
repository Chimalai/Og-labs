
# Og-labs
script to automate image uploads to the 0G (Zero Gravity) testnet decentralized storage, supporting multiple wallets and proxy rotation for enhanced reliability and privacy.

## Features

- **Automated uploads:** Uploads random images to the 0G decentralized storage network.
- **Multiple wallet support:** Use multiple private keys for batch operations.
- **Proxy rotation:** Supports rotating proxy servers to avoid rate limits and enhance privacy.


### Installation

1. **Clone this repository:**
   ```sh
   git clone https://github.com/Chimalai/Og-labs.git
   cd Og-labs
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Configure environment variables:**
   - Copy the example `.env` file and fill in your private key(s):
     ```sh
     cp .env.example .env
     ```
   - Edit `.env` and add your wallet private keys:
     ```
     PRIVATE_KEY_1=0xyourprivatekey1here
     PRIVATE_KEY_2=0xyourprivatekey2here
     # Add more as needed
     ```

4. **(Optional) Add proxies:**
   - Create a `proxies.txt` file in the project root.
   - List one proxy per line (format: `http://user:pass@host:port` or `http://host:port`).

### Usage

Run the main script:

```sh
node index.js
```

- You will be prompted for the number of files to upload per wallet.
- The script will process uploads, print transaction info, and provide a summary at the end.

### Example

```
[INFO] Loaded 2 private key(s).
[INFO] Loaded 5 proxies from proxies.txt.
[LOADING] Checking network status...
[SUCCESS] Connected to network: chainId 16601
...
[SUMMARY] Total wallets: 2
[SUMMARY] Uploads per wallet: 3
[SUMMARY] Total attempts: 6
[SUCCESS] Successful uploads: 6
[SUCCESS] All operations completed.
[INFO] Process finished.
```

## Environment Variables

Set your private keys in the `.env` file:

```env
PRIVATE_KEY_1=0x...
PRIVATE_KEY_2=0x...
```

## Proxy Support

- Add your proxies to `proxies.txt` (one per line).
- If no proxies are provided, uploads will use your direct connection.

## Security

**Never share your private keys or `.env` file.**  
Add `.env` and `proxies.txt` to your `.gitignore` to keep them out of version control.

## License

This project is licensed under the MIT License.

---

```
## Support

## If you want to buy me coffee
```
0x6b09F6E036E83a7F12530Ea96aC25e73090DFF8C
```
