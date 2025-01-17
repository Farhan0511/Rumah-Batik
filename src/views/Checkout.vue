<template>

    <div>
        <navbar/>
    </div>

    <div class="container mt-5">
        <h2 class="text-center mb-4">Checkout</h2>
    </div>
    
    <div class="container">

        <div class="container m-5">
            <form>
                <div class="row">
                    <!-- Billing Details -->
                    <div class="col-md-6">
                        <h4>Billing Details</h4>
                        <div class="mb-3">
                            <label for="fullName" class="form-label">Full Name</label>
                            <input type="text" class="form-control" id="fullName" placeholder="Enter your full name">
                        </div>
                        <div class="mb-3">
                            <label for="email" class="form-label">Email Address</label>
                            <input type="email" class="form-control" id="email" placeholder="Enter your email">
                        </div>
                        <div class="mb-3">
                            <label for="phone" class="form-label">Phone Number</label>
                            <input type="text" class="form-control" id="phone" placeholder="Enter your phone number">
                        </div>
                        <div class="mb-3">
                            <label for="address" class="form-label">Address</label>
                            <textarea class="form-control" id="address" rows="3"
                                placeholder="Enter your address"></textarea>
                        </div>
                    </div>

                    <!-- Order Summary -->
                    <div class="col-md-6">
                        <h4>Order Summary</h4>
                        <ul class="list-group mb-3">
                            <li class="list-group-item d-flex justify-content-between">
                                <span>Product 1</span>
                                <strong>$50</strong>
                            </li>
                            <li class="list-group-item d-flex justify-content-between">
                                <span>Product 2</span>
                                <strong>$30</strong>
                            </li>
                            <li class="list-group-item d-flex justify-content-between">
                                <span>Shipping</span>
                                <strong>$10</strong>
                            </li>
                            <li class="list-group-item d-flex justify-content-between">
                                <strong>Total</strong>
                                <strong>$90</strong>
                            </li>
                        </ul>
                        <div class="mb-3">
                            <label for="paymentMethod" class="form-label">Payment Method</label>
                            <select class="form-select" id="paymentMethod">
                                <option value="credit-card">Credit Card</option>
                                <option value="paypal">PayPal</option>
                                <option value="bank-transfer">Bank Transfer</option>
                            </select>
                        </div>
                    </div>
                </div>

                <!-- Submit Button -->
                <div class="text-center mt-4">
                    <button type="submit" class="btn btn-primary btn-lg">Place Order</button>
                </div>
            </form>
        </div>



    </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue';

export default {
    name: "CheckOut",
    components: {
        Navbar
    }
}
</script>

<style></style>