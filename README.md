// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract AuctionWinner {
    address public winner;

    function setWinner(address _winner) external {
        winner = _winner;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract RefundStyle {
    bool public refundable;

    function enableRefunds() external {
        refundable = true;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract RewardRate {
    uint256 public rate = 100; // example rate

    function setRate(uint256 _rate) external {
        rate = _rate;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CompoundFlag {
    mapping(address => bool) public autoCompound;

    function setCompound(bool enabled) external {
        autoCompound[msg.sender] = enabled;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CompoundFlag {
    mapping(address => bool) public autoCompound;

    function setCompound(bool enabled) external {
        autoCompound[msg.sender] = enabled;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract NFTBurn {
    mapping(uint256 => bool) public burned;

    function burn(uint256 tokenId) external {
        burned[tokenId] = true;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract TokenExists {
    mapping(uint256 => bool) public exists;

    function mint(uint256 tokenId) external {
        exists[tokenId] = true;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract MarketplaceFee {
    uint256 public feeBps = 250; // 2.5%

    function setFee(uint256 bps) external {
        feeBps = bps;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CollectionSize {
    uint256 public maxSupply = 10000;

    function setMaxSupply(uint256 _max) external {
        maxSupply = _max;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract MaxPerWallet {
    uint256 public maxPerWallet = 5;

    function setMax(uint256 _max) external {
        maxPerWallet = _max;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract BaseURI {
    string public baseURI;

    function setBaseURI(string calldata uri) external {
        baseURI = uri;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract OperatorFilter {
    mapping(address => bool) public blockedOperators;

    function blockOperator(address operator) external {
        blockedOperators[operator] = true;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Attributes {
    mapping(uint256 => uint256) public attributeCount;

    function setAttributes(uint256 tokenId, uint256 count) external {
        attributeCount[tokenId] = count;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Attributes {
    mapping(uint256 => uint256) public attributeCount;

    function setAttributes(uint256 tokenId, uint256 count) external {
        attributeCount[tokenId] = count;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Cooldown {
    mapping(address => uint256) public cooldownUntil;

    function startCooldown(uint256 duration) external {
        cooldownUntil[msg.sender] = block.timestamp + duration;
    }
}
