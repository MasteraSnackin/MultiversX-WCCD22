Explanation
Character Struct: Represents the character with attributes for defense and attack.

equipTool Endpoint: Allows users to equip a tool (like a Sword or Shield) to a character. The tool NFT is consumed, and the character's attributes are updated based on the tool type.

Helper Functions:

is_owner_of_nft: Verifies that the caller owns the specified NFTs.
consume_nft: Handles consuming or burning the tool NFT after it has been used.
Documentation
Smart Contract Design: The contract is designed to manage characters and tools as NFTs. Users can equip tools to their characters to enhance specific attributes. The tool NFT is consumed in the process to prevent reuse.

Verification: The contract's logic is explicit and verifiable by examining the code and ABI, ensuring transparency in how NFTs are managed and attributes are updated.

Open Source: The contract is intended to be open source, allowing others to review, use, and contribute to its development.

Deployment and Usage
Build the Contract: Compile the smart contract to WebAssembly.

cargo build --release --target=wasm32-unknown-unknown
Deploy the Contract: Use MultiversX tools to deploy the compiled Wasm file to the MultiversX Devnet or Mainnet.

Interact with the Contract: Use the MultiversX Devnet Explorer or CLI to call endpoints such as equipTool.