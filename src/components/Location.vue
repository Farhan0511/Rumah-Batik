<template>
   <div class="container mt-5">
    <div class="p-4 bg-light shadow-sm rounded">
        <div class="row">
            <!-- Our Location Section -->
            <div class="col-lg-6">
                <div class="text-center mb-4">
                    <h2 class="fw-bold">Our Location</h2>
                </div>
                <div class="ratio ratio-16x9">
                    <iframe
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d31737.193305308145!2d106.13842036174573!3d-6.110610486078495!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e418b0dbb534a61%3A0x301e8f1fc28b8d0!2sSerang%2C%20Kec.%20Serang%2C%20Kota%20Serang%2C%20Banten!5e0!3m2!1sid!2sid!4v1736481726240!5m2!1sid!2sid"
                        style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>

            <!-- Criticism and Suggestions Section -->
            <div class="col-lg-6">
                <div class="card shadow-sm">
                    <div class="card-body">
                        <h3 class="card-title text-center mb-4 fw-bold">Criticism and suggestions!</h3>

                        <!-- Username -->
                        <div class="mb-3">
                            <label for="username" class="form-label">Email</label>
                            <div class="input-group">
                                <input type="text" class="form-control" id="username" placeholder="example@gmail.com"
                                    aria-label="Username" aria-describedby="basic-addon1">
                            </div>
                        </div>

                        <!-- Amount -->
                        <div class="mb-3">
                            <label for="username" class="form-label">No WA</label>
                            <div class="input-group">
                                <input type="text" class="form-control" id="nowa" placeholder="+62"
                                    aria-label="Username" aria-describedby="basic-addon1">
                            </div>
                        </div>

                        <!-- Textarea -->
                        <div class="mb-3">
                            <label for="textarea" class="form-label">Message</label>
                            <div class="input-group">
                                <textarea class="form-control" id="textarea" aria-label="With textarea" placeholder="Very Cool!"></textarea>
                            </div>
                        </div>

                        <!-- Submit Button -->
                        <div class="d-grid">
                            <button type="button" class="btn btn-primary btn-lg">Submit</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>
export default {
    name: "LocationPage"
}
</script>

<style></style>