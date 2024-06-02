// create a variable to hold your NFT's
let nftCollection = [];
// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT (id, name, game, place , university) {
    let newNFT ={
        id: id,
        name: name,
        game: game,
        place: place,
        university: university,
    }
    nftCollection.push(newNFT);
}

// create a "loop" that will go through an "array" of NFT's
// and print their metadata with console.log()
function listNFTs () {
    for(let m = 0; m < nftCollection.length; m++){
        let nft = nftCollection[m];
        console.log("NFT ID: " + nft.id + " ,Name:" + nft.name + " ,Game:" + nft.game + " ,Place:" + nft.place + " ,University:" + nft.university) ;
    }
}

// print the total number of NFTs we have minted to the console
function getTotalSupply() {
    console.log("Total no of NFT: " + nftCollection.length);
}

mintNFT(1, "Amit", "UFC", "chandigarh", "stanford")
// call your functions below this line
listNFTs();
getTotalSupply();











