<template>
    <div class="content bg-slate-300">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.2/css/all.min.css"
            integrity="sha512-1sCRPdkRXhBV2PBLUdRb4tMg1w2YPf37qatUFeS7zlBy7jJI8Lf4VHwWfZZfpXtYSLy85pkm9GaYVYMfw5BC1A=="
            crossorigin="anonymous" referrerpolicy="no-referrer" />



        <div class="border-solid border-2 border-black drop-shadow-md bg-gray-300">
            <form>
                <h1 style="color:darkslateblue" class="font-bold  text-2xl">Product List</h1>
                <table>
                    <tr class="text-center">
                        <td><label>Product Name :</label></td>
                        <td><input type="text" v-model="formdata.pname"
                                class="bg-white border border-slate-300 rounded-md py-2 pl-9 pr-3 m-5"></td>
                    </tr>
                    <tr>
                        <td><label>Product Price :</label></td>
                        <td><input type="text" v-model="formdata.price"
                                class="bg-white border border-slate-300 rounded-md py-2 pl-9 pr-3 m-5"></td>
                    </tr>
                    <tr>
                        <td><label>Product Category:</label></td>
                        <td><input type="text" v-model="formdata.category"
                                class="bg-white border border-slate-300 rounded-md py-2 pl-9 pr-3 m-5"></td>
                    </tr>
                    <tr>
                        <td><label>Product Color :</label></td>
                        <td><input type="text" v-model="formdata.color"
                                class="bg-white border border-slate-300 rounded-md py-2 pl-9 pr-3 m-5"></td>
                    </tr>
                    <tr>
                        <td>
                            <button type="button"
                                class=" border-solid font-extrabold rounded border-2 border-black p-3 bg-gray-300 bg-hover-black"
                                @click="login">
                                <NuxtLink to="/productForm"> Submit </NuxtLink>
                            </button>
                        </td>
                    </tr>
                </table>
            </form>
        </div>







        <h1 class="text-center font-extrabold text-5xl mt-8 bg-blue-200">Product List</h1>

        <nav class="text-center font-bold text-xl mt-8 ">
            <a>
                <select name="Category" id="jeans" class="bg-gray-300">
                    <option value="jeans"></option>
                    <option value="jeans">Regular</option>


                </select>

                <select name="Category" id="Tshirt" class="bg-gray-300">
                    <option value="Tshirt">Bags</option>
                    <option value="Tshirt">Travelling</option>
                    <option value="Tshirt">school</option>
                    <option value="Tshirt">Army</option>
                    <option value="Tshirt">Side-Bag</option>
                </select>


                <select name="Category" id="HAT" class="bg-gray-300">
                    <option value="">Select HAT</option>
                    <option value="earphone">Round</option>
                    <option value="earphone">cow</option>

                </select>
                <select name="Category" id="shoes" class="bg-gray-300">
                    <option value="shoes">Select Shoes</option>
                    <option value="shoes">Formal Shoes</option>
                    <option value="shoes">Casual Shoes</option>
                </select><br>
                <div class="inline-flex p-4 mt-4">
                    <div class="mr-8 border-2 px-2 border-black rounded-md"><a href="productform">Add Products</a></div>
                    <div class="ml-8 border-2 px-2 border-black rounded-md"><a href="mainform2">Shoe Category</a></div>
                </div>
            </a>
        </nav>
        <div>
            <table class="mt-6">
                <tr class="border-2 rounded-md border-black">
                    <td class="text-center p-2">
                        <div>
                            <img src="RoundNeck.jpg" alt="showimage" class=" pl-56 items-center">
                            <p></p>
                            <h3 class="font-bold text-xl">T-Shirt</h3>
                            <p><b>Round</b></p>
                            <h5><b>Rs 10,000/-only</b></h5>
                            <!-- <p><input type="color"/>color</p> -->
                            <div>
                                <label for="color">Choose color:</label>

                                <select name="Colors" id="color">
                                    <option value="White">White</option>
                                    <option value="Blue">Blue</option>
                                    <option value="Red">Red</option>
                                    <option value="Green">Green</option>
                                </select>
                            </div>

                            <button></button>
                            <i class="fa fa-star checked"></i><i class="fa fa-star checked"></i><i
                                class="fa fa-star checked"></i><br>
                            <button class="buy-1 border-2 px-2  border-black rounded-md">Buy Now</button>
                        </div>
                    </td>
                    <td class="p-2">
                        <div class="content text-center ">
                            <img src="vneck.jpg" alt="showimage" class="px-64 items-center ">
                            <h3 class="font-bold text-xl">Tshirt</h3>
                            <p><b>V-Neck</b></p>
                            <h5><b>Rs 11,200/-only</b></h5>
                            <div>
                                <label for="color">Choose color:</label>

                                <select name="Colors" id="color">
                                    <option value="White">White</option>
                                    <option value="Blue">Blue</option>
                                    <option value="Red">Red</option>
                                    <option value="Green">Green</option>
                                </select>
                            </div>
                            <i class="fa fa-star checked"></i><i class="fa fa-star checked"></i><i
                                class="fa fa-star checked"></i><br>
                            <button class="buy-2 border-2 px-2  border-black rounded-md">Buy Now</button>
                        </div>
                    </td>
                </tr>
                <tr class="border-2 rounded-md border-black">
                    <td class="p-2">
                        <div class="content text-center">
                            <img src="chapri.jpg" alt="showimage" class="px-64  items-center">
                            <h3 class="font-bold text-xl">T-Shirt</h3>
                            <p><b>Chapri</b></p>
                            <h5><b>Rs 11,500/- only</b></h5>
                            <div>
                                <label for="color">Choose color:</label>

                                <select name="Colors" id="color">
                                    <option value="White">White</option>
                                    <option value="Blue">Blue</option>
                                    <option value="Red">Red</option>
                                    <option value="Green">Green</option>
                                </select>
                            </div>
                            <i class="fa fa-star checked"></i><i class="fa fa-star checked"></i><i
                                class="fa fa-star checked"></i><br>
                            <button class="buy-3 border-2 px-2  border-black rounded-md">Buy Now</button>
                        </div>
                    </td>
                    <td class="p-2">
                        <div class="content text-center h-3">
                            <img src="beneton.jpg" alt="showimage" class="px-64  items-center">
                            <h3 class="font-bold text-xl">T-Shirt</h3>
                            <p><b>United colors oif Beneton</b></p>
                            <h5><b>Rs 13,200/- only</b></h5>
                            <div>
                                <label for="color">Choose color:</label>

                                <select name="Colors" id="color">
                                    <option value="White">White</option>
                                    <option value="Blue">Blue</option>
                                    <option value="Red">Red</option>
                                    <option value="Green">Green</option>
                                </select>
                            </div>
                            <i class="fa fa-star checked"></i><i class="fa fa-star checked"></i><i
                                class="fa fa-star checked"></i><br>
                            <button class="buy-4 border-2 px-2  border-black rounded-md">Buy Now</button>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

    </div>
</template>


<script>
export default {
    name: 'formdataproduct',
    data() {
        return {
            myarr: [],
            formdata: {
                pname: "",
                price: "",
                category: "",
                color: "",
                image : "",
            },
        };
    },
    methods: {
        createNewCard() {
            this.myarr.push(this.formdata);
        },
        login(event) {
            event.preventDefault();
            if (this.isEdit == true) {
                this.myarr[this.indexEdit] = this.formdata;
                this.isEdit = false;
                this.indexEdit = -1;
            } else {
                this.myarr.push(this.formdata);
            }
            this.formdata = {
                id: 0,
                pname: "",
                price: "",
                category: "",
                color: "",
                image : "",
            }
            console.log("Formdata is :", this.myarr);
        },
        deleteIndex(index) {
            this.myarr.splice(index, 1);
        },
        editIndex(index) {
            this.formdata.pname = this.myarr[index].pname;
            this.formdata.price = this.myarr[index].price;
            this.formdata.category = this.myarr[index].category;
            this.formdata.color = this.myarr[index].color;
            this.formdata.image = this.myarr[index].image;
            this.isEdit = true;
            this.indexEdit = index;
        },
    }
}
</script>

