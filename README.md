    private fun loadTestData() {
        val baseItem = BaseItem(
            id = 1,
            name = "Pizza",
            price = 10,
            description = "Delicious pizza with your choice of toppings",
            groups = listOf(
                Group(
                    id = 101,name = "Crust",
                    addons = listOf(
                        Addon(
                            id = 201,
                            name = "Thin Crust",
                            price = 0.0,
                            groups = listOf(
                                Group(
                                    id = 301,
                                    name = "Extra Thin",
                                    addons = listOf(
                                        Addon(
                                            id = 401,
                                            name = "Double Thin",
                                            price = 2.0,
                                            groups = null
                                        )
                                    )
                                ),
                                Group(
                                    id = 301,
                                    name = "Medium Thin",
                                    addons = listOf(
                                        Addon(
                                            id = 401,
                                            name = "Medium Thin",
                                            price = 2.0,
                                            groups = null
                                        )
                                    )
                                )
                            )
                        ),
                        Addon(
                            id = 202,
                            name = "Thick Crust",
                            price = 1.0,
                            groups = listOf(
                                Group(
                                id = 301,
                                name = "Extra Thick",
                                addons = listOf(
                                    Addon(
                                        id = 401,
                                        name = "Double Thick",
                                        price = 2.0,
                                        groups = null
                                    )
                                )
                            ),
                                Group(
                                    id = 301,
                                    name = "Medium Thick",
                                    addons = listOf(
                                        Addon(
                                            id = 401,
                                            name = "Medium Thick",
                                            price = 2.0,
                                            groups = null
                                        )
                                    )
                                )
                            )
                        )
                    )
                ),
                Group(
                    id = 102,
                    name = "Toppings",
                    addons = listOf(
                        Addon(
                            id =211,
                            name = "Pepperoni",
                            price = 1.5,
                            groups = listOf(
                                Group(
                                    id = 301,
                                    name = "Extra Pepperoni",
                                    addons = listOf(
                                        Addon(
                                            id = 401,
                                            name = "Double Pepperoni",
                                            price = 2.0,
                                            groups = null
                                        )
                                    )
                                )
                            )
                        ),
                        Addon(
                            id = 212,
                            name = "Mushrooms",
                            price = 1.0,
                            groups = null
                        )
                    )
                )
            ),
            variants = listOf(
                Variant(
                    id = 10,
                    name = "Vegetarian Pizza",
                    priceAdjustment = -1,
                    groups = listOf(
                        Group(
                            id = 111,
                            name = "Veggie Toppings",
                            addons = listOf(
                                Addon(
                                id = 221,
                                name = "Onions",
                                price = 0.5,
                                groups = listOf(
                                    Group(
                                        id = 311,
                                        name = "Spicy Onions",
                                        addons = listOf(
                                            Addon(
                                                id = 411,
                                                name = "Jalapenos",
                                                price = 0.25,
                                                groups = null
                                            )
                                        )
                                    ), Group(
                                        id = 311,
                                        name = "Sweet Onions",
                                        addons = listOf(
                                            Addon(
                                                id = 411,
                                                name = "Jalapenos",
                                                price = 0.25,
                                                groups = null
                                            )
                                        )
                                    )
                                )
                            ),
                                Addon(
                                    id = 222,
                                    name = "Green Peppers",
                                    price = 0.75,
                                    groups = listOf(
                                        Group(
                                            id = 311,
                                            name = "Spicy Peppers",
                                            addons = listOf(
                                                Addon(
                                                    id = 411,
                                                    name = "Jalapenos",
                                                    price = 0.25,
                                                    groups = null
                                                )
                                            )
                                        )
                                    )
                                )
                            )
                        ),
                        Group(
                            id = 111,
                            name = "Panner Toppings",
                            addons = listOf(
                                Addon(
                                    id = 221,
                                    name = "Paneer Onions",
                                    price = 0.5,
                                    groups = listOf(
                                        Group(
                                            id = 311,
                                            name = "Paneer Onions",
                                            addons = listOf(
                                                Addon(
                                                    id = 411,
                                                    name = " Paneer Jalapenos",
                                                    price = 0.25,
                                                    groups = null
                                                )
                                            )
                                        ), Group(
                                            id = 311,
                                            name = "Paneer Sweet Onions",
                                            addons = listOf(
                                                Addon(
                                                    id = 411,
                                                    name = "Jalapenos",
                                                    price = 0.25,
                                                    groups = null
                                                )
                                            )
                                        )
                                    )
                                )
                            )
                        )

                    )
                ),
                Variant(
                    id = 11,
                    name = "Non Vegetarian Pizza",
                    priceAdjustment = -1,
                    groups = listOf(
                        Group(
                            id = 112,
                            name = "Non Veggie Toppings",
                            addons = listOf(
                                Addon(
                                id = 2211,
                                name = "Non Onions",
                                price = 0.5,
                                groups = null
                            ),
                                Addon(
                                    id = 2221,
                                    name = "Non Green Peppers",
                                    price = 0.75,
                                    groups = listOf(
                                        Group(
                                            id = 3111,
                                            name = "Non Spicy Peppers",
                                            addons = listOf(
                                                Addon(
                                                    id = 411,
                                                    name = "Jalapenos",
                                                    price = 0.25,
                                                    groups = null
                                                )
                                            )
                                        )
                                    )
                                )
                            )
                        )
                    )
                )
            )
        )

        val testData = TestData(baseItem)
        _testData.value = testData
    }


This  is the data set used 
