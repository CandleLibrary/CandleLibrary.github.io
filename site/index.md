<import template url="./fp_template.wick"></import>
<import name="libraries" url="./libraries.json"></import>

<div class="cta">
<md>

# The Candle Library 

<button> Getting Started </button> <button> Support </button>

</md>
</div>


## Modern Libraries for the Modern Developer

## Philosophy

- Easy to use, hard to break.
    - Flexible: Stand alone architecture
    - If it feels like something is hard, we need to modify, remove, or extend the module to make it easy.

- Painfully Obvious: If you think something will work a certain way, it probably will.

- Informative: The moment we don't have an answer for you, is the moment you have enough information to create the answere yourself.

## Core Libraries


<container class="library-section" data={ libraries }>
    <div class="doc-section">
        <h2> {name} </h2>
        <p> Some Text about this library </a>
        <a href={"https://" + repo}><button>docs</button></a>
        <a href={"https://" + repo}><button>github</button></a>
    </div>
</container>

<style>
    .cta {
        width:100%;
        height:100vh;
    }

    .library-section{
        width:100%;
        display:grid;
        grid-template-columns: 50% 50%;
    }

    .doc-section {
        padding:50px;
        margin:20px;
        min-height: 120px;
        border: 1px solid #BBB;
        border-radius:5px;
    }

    .doc-section * {
        margin-left:20px;
    }

    root > h2, root > h3 {
        text-align:center
    }

    .doc-section h2 {
        margin:0;
        text-align:left;
    }

    button {
        min-width: 90px;
        height: 50px;
        margin: 10px 15px;
        border-radius:5px;
        border:2px solid rgb(22,120,220);
        background-color:transparent;
        transition: 300ms all;
    }

    button:hover{
        cursor:pointer;
        border:2px solid rgb(225,120,150);
    }
</style>