<template>
 <div class="crypto">
    <div class="overflow-x-auto">
        <div class="min-w-screen min-h-screen bg-gray-100 flex items-center justify-center bg-gray-100 font-sans overflow-hidden">
            <div class="w-full lg:w-5/6">
                <div class="bg-white shadow-md rounded my-6">
                    <table class="min-w-max w-full table-auto">
                        <thead>
                            <tr class="bg-gray-200 text-gray-600 uppercase text-sm leading-normal">
                                <th class="py-3 px-6 text-left">#</th>
                                <th class="py-3 px-6 text-left"></th>
                                <th class="py-3 px-6 text-center">Name</th>
                                <th class="py-3 px-6 text-center">Market Cap</th>
                                <th class="py-3 px-6 text-center">Price ($)</th>
                                <th class="py-3 px-6 text-center">Change</th>
                                <th class="py-3 px-6 text-center">Volume ($)</th>
                                <th class="py-3 px-6 text-center">Algorithm</th>
                            </tr>
                        </thead>
                        <tbody class="text-gray-600 text-sm font-light">
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                              <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <span>1</span>
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <img src="https://localbitcoinnow.com/wp-content/uploads/2019/12/The-bit-logo-e1575819611411.png"
                                                 width="24" height="24"
                                                 style=" fill:#000000;" />
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>Bitcoin (BTC)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>594,986,672,698</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-white-600 py-1 px-3 rounded-full text-xs">31,665.01</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-white-600 py-1 px-3 rounded-full text-xs">+172.57(0.55%)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>2,596,857,820.61</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>SHA-256d</span>
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                              <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <span>2</span>
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <img src="https://res.cloudinary.com/teepublic/image/private/s--UbaxRjB3--/c_crop,x_10,y_10/c_fit,h_830/c_crop,g_north_west,h_1038,w_1038,x_-264,y_-104/l_upload:v1565806151:production:blanks:vdbwo35fw6qtflw9kezw/fl_layer_apply,g_north_west,x_-375,y_-215/b_rgb:262c3a/c_limit,f_jpg,h_630,q_90,w_630/v1470823069/production/designs/625723_1.jpg"
                                                 width="24" height="24"
                                                 style=" fill:#000000;" />
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>Ethereum (ETH)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>222,588,945,933</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-white-600 py-1 px-3 rounded-full text-xs">1,900.64</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-green-200 text-white-600 py-1 px-3 rounded-full text-xs">+12.56(0.67%)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>2,206,626,116.61</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>Ethash</span>
                                </td>
                            </tr>
                            <tr class="border-b border-gray-200 hover:bg-gray-100">
                              <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <span>3</span>
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-left whitespace-nowrap">
                                    <div class="flex items-center">
                                        <div class="mr-2">
                                            <img src="data:image/jpeg;base64,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"
                                                 width="24" height="24"
                                                 style=" fill:#000000;" />
                                        </div>
                                    </div>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>Tether USD (USDT)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>62,201,249,596</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-red-200 text-white-600 py-1 px-3 rounded-full text-xs">0.970</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span class="bg-red-200 text-white-600 py-1 px-3 rounded-full text-xs">+-0.030(-3.00%)</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>74,592,816.56</span>
                                </td>
                                <td class="py-3 px-6 text-center">
                                    <span>Not Mineable/Ethereum</span>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>s
  </div>
</template>

<script>
export default {}
</script>

<style>
</style>