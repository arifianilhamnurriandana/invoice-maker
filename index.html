<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title class="hidden">Invoice Generator</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <style>
        /* Styling khusus untuk print */
        @media print {
            body * {
                visibility: hidden;
            }

            .print-invoice,
            .print-invoice * {
                visibility: visible;
            }

            .print-invoice {
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
            }

            .invoice-container {
                padding: 20px;
                font-family: Arial, sans-serif;
                color: #333;
            }

            .invoice-header {
                text-align: center;
                margin-bottom: 20px;
            }

            .invoice-title {
                font-size: 24px;
                font-weight: bold;
                margin-bottom: 10px;
            }

            .invoice-info {
                display: flex;
                justify-content: space-between;
                margin-bottom: 20px;
            }

            .invoice-info div {
                width: 48%;
            }

            .invoice-details,
            .invoice-footer {
                width: 100%;
                margin-top: 20px;
            }

            .invoice-table {
                width: 100%;
                border-collapse: collapse;
            }

            .invoice-table th,
            .invoice-table td {
                border: 1px solid #ccc;
                padding: 10px;
                text-align: left;
            }

            .invoice-table th {
                background-color: #f5f5f5;
            }

            .text-right {
                text-align: right;
            }

            .text-center {
                text-align: center;
            }

            .total-section {
                margin-top: 20px;
                font-weight: bold;
            }

            .no-print {
                display: none;
            }
        }
    </style>
</head>

<body class="bg-gray-100 p-6">

    <div class="max-w-3xl mx-auto bg-white p-8 rounded-lg shadow-lg">
        <h2 class="font-bold mb-4 no-print">Invoice Generator</h2>

        <div class="grid grid-cols-2 gap-4 mb-6">
            <div>
                <label for="namaPembuat" class="block text-sm font-medium text-gray-700">Nama Pembuat</label>
                <input type="text" id="namaPembuat" class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
            </div>
            <div>
                <label for="namaPelanggan" class="block text-sm font-medium text-gray-700">Nama Pelanggan</label>
                <input type="text" id="namaPelanggan" class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
            </div>
            <div>
                <label for="tanggalPembuatan" class="block text-sm font-medium text-gray-700">Tanggal Pembuatan</label>
                <input type="date" id="tanggalPembuatan"
                    class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
            </div>
            <div>
                <label for="alamatPembuat" class="block text-sm font-medium text-gray-700">Alamat Pembuat</label>
                <input type="text" id="alamatPembuat" class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
            </div>
            <div>
                <label for="alamatPelanggan" class="block text-sm font-medium text-gray-700">Alamat Pelanggan</label>
                <input type="text" id="alamatPelanggan" class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
            </div>
            <div>
                <label for="kodeInvoice" class="block text-sm font-medium text-gray-700">Kode Invoice</label>
                <input type="text" id="kodeInvoice" class="mt-1 block w-full p-2 border border-gray-300 rounded-md"
                    value="" disabled>
            </div>
        </div>

        <div class="mb-6">
            <label for="namaProduk" class="block text-sm font-medium text-gray-700">Nama Produk</label>
            <input type="text" id="namaProduk" class="mt-1 block w-full p-2 border border-gray-300 rounded-md">
        </div>
        <div class="mb-6">
            <label for="deskripsiProduk" class="block text-sm font-medium text-gray-700">Deskripsi Produk</label>
            <textarea id="deskripsiProduk" class="mt-1 block w-full p-2 border border-gray-300 rounded-md"></textarea>
        </div>
        <div class="grid grid-cols-3 gap-4 mb-6">
            <div>
                <label for="hargaProduk" class="block text-sm font-medium text-gray-700">Harga Produk</label>
                <input type="number" id="hargaProduk" class="mt-1 block w-full p-2 border border-gray-300 rounded-md"
                    oninput="updateTotal()">
            </div>
            <div>
                <label for="jumlahProduk" class="block text-sm font-medium text-gray-700">Jumlah Produk</label>
                <input type="number" id="jumlahProduk" class="mt-1 block w-full p-2 border border-gray-300 rounded-md"
                    oninput="updateTotal()">
            </div>
            <div>
                <label for="totalHarga" class="block text-sm font-medium text-gray-700">Total Harga</label>
                <input type="text" id="totalHarga" class="mt-1 block w-full p-2 border border-gray-300 rounded-md"
                    disabled>
            </div>
        </div>

        <button onclick="generateInvoice()" class="bg-blue-500 text-white px-4 py-2 rounded">Generate Invoice</button>
    </div>

    <div class="print-invoice max-w-3xl mx-auto bg-white p-8 rounded-lg shadow-lg invoice-container mt-8 hidden">
        <div class="invoice-header">
            <h1 class="invoice-title" id="invoiceTitle">TAGIHAN</h1>
            <p>TANGGAL PEMBUATAN: <span id="tanggalPembuatanPrint"></span></p>
        </div>

        <div class="invoice-info">
            <div>
                <p>TAGIHAN DARI:</p>
                <p id="namaPembuatPrint"></p>
                <p id="alamatPembuatPrint"></p>
            </div>
            <div>
                <p>KEPADA:</p>
                <p id="namaPelangganPrint"></p>
                <p id="alamatPelangganPrint"></p>
            </div>
        </div>

        <div class="invoice-details">
            <table class="invoice-table">
                <thead>
                    <tr>
                        <th>DESKRIPSI</th>
                        <th>KUANTITAS</th>
                        <th>HARGA</th>
                        <th>JUMLAH</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td id="namaProdukPrint"></td>
                        <td class="text-center" id="jumlahProdukPrint"></td>
                        <td class="text-right" id="hargaProdukPrint"></td>
                        <td class="text-right" id="jumlahHargaPrint"></td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="total-section text-right">
            <p>TOTAL: <span id="totalHargaPrint"></span></p>
        </div>

        <div class="invoice-footer text-center">
            <p>My Invoice - Professional Invoice</p>
        </div>

        <div class="text-center mt-4" id="printButton">
            <button onclick="window.print()" class="bg-green-500 text-white px-4 py-2 rounded">Print Invoice</button>
        </div>
    </div>
    <script>
        function generateRandomCode(prefix, length) {
            let result = prefix;
            const characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789';
            const charactersLength = characters.length;
            let counter = 0;
            while (counter < length) {
                result += characters.charAt(Math.floor(Math.random() * charactersLength));
                counter += 1;
            }
            return result;
        }

        function updateTotal() {
            const hargaProduk = parseFloat(document.getElementById('hargaProduk').value) || 0;
            const jumlahProduk = parseInt(document.getElementById('jumlahProduk').value) || 0;
            const totalHarga = hargaProduk * jumlahProduk;
            document.getElementById('totalHarga').value = 'Rp ' + totalHarga.toLocaleString('id-ID');
        }

        function generateInvoice() {
            const namaPembuat = document.getElementById('namaPembuat').value;
            const namaPelanggan = document.getElementById('namaPelanggan').value;
            const tanggalPembuatan = document.getElementById('tanggalPembuatan').value;
            const alamatPembuat = document.getElementById('alamatPembuat').value;
            const alamatPelanggan = document.getElementById('alamatPelanggan').value;
            const kodeInvoice = generateRandomCode('JPW', 5); // Contoh kode dengan awalan 'JPW' dan panjang 5 karakter acak
            const namaProduk = document.getElementById('namaProduk').value;
            const deskripsiProduk = document.getElementById('deskripsiProduk').value;
            const hargaProduk = parseFloat(document.getElementById('hargaProduk').value) || 0;
            const jumlahProduk = parseInt(document.getElementById('jumlahProduk').value) || 0;
            const totalHarga = hargaProduk * jumlahProduk;

            document.getElementById('kodeInvoice').value = kodeInvoice;
            document.getElementById('invoiceTitle').innerText = `TAGIHAN ${kodeInvoice}`;
            document.getElementById('namaPembuatPrint').innerText = namaPembuat;
            document.getElementById('namaPelangganPrint').innerText = namaPelanggan;
            document.getElementById('tanggalPembuatanPrint').innerText = tanggalPembuatan;
            document.getElementById('alamatPembuatPrint').innerText = alamatPembuat;
            document.getElementById('alamatPelangganPrint').innerText = alamatPelanggan;

            document.getElementById('namaProdukPrint').innerText = namaProduk + " - " + deskripsiProduk;
            document.getElementById('jumlahProdukPrint').innerText = jumlahProduk;
            document.getElementById('hargaProdukPrint').innerText = 'Rp ' + hargaProduk.toLocaleString('id-ID');
            document.getElementById('jumlahHargaPrint').innerText = 'Rp ' + totalHarga.toLocaleString('id-ID');
            document.getElementById('totalHargaPrint').innerText = 'Rp ' + totalHarga.toLocaleString('id-ID');

            document.querySelector('.print-invoice').classList.remove('hidden');
            document.getElementById('printButton').classList.remove('hidden');
        }
        function printInvoice() {
            // Sembunyikan elemen yang tidak ingin dicetak
            document.querySelector('.no-print').style.display = 'none';

            // Cetak halaman
            window.print();

            // Tampilkan kembali elemen setelah mencetak
            document.querySelector('.no-print').style.display = '';
        }
    </script>

</body>

</html>
