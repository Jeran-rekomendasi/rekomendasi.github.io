<!--  code html untuk memilih kriteria pengurutan -->
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rekomendasi Film</title>
    <link rel="stylesheet" href="css/style.css">
</head>

<body>
    <form method="get" action="">
        <label for="sort">Urutkan Berdasarkan:</label>
        <select name="sort" id="sort">
            <option value="rating">Rating</option>
            <option value="popularitas">Popularitas</option>
            <option value="tahun_rilis">Tahun Rilis</option>
        </select>
        <button type="submit">Urutkan</button>
    </form>

    <form method="GET" action="">
        <label for="genre">Pilih Genre:</label>
        <select name="genre" id="genre">
            <option value="">Semua Genre</option>
            <option value="Action">Action</option>
            <option value="Drama">Drama</option>
            <option value="Komedi">Komedi</option>
            <option value="Horror">Horror</option>
            <option value="Sci-Fi">Sci-Fi</option>
        </select>
        <input type="submit" value="Tampilkan">
    </form>


    <!-- code php -->
    <?php
    // Menghubungkan mysql dengan php
    $conn = new mysqli(
        "localhost",
        "root",
        "",
        "rekomendasi_film"
    );
    if ($conn->connect_error) {
        die("Koneksi database gagal: " . $conn->connect_error);
    }
    // Mengambil data film
    $sql = "SELECT * FROM film";
    $result = $conn->query($sql);
    $data = [];
    if ($result->num_rows > 0) {
        while ($row = $result->fetch_assoc()) {
            $data[] = $row;
        }
    }
    $conn->close();

    // Mengambil pilihan genre dari form
    $selectedGenre = isset($_GET['genre']) ? $_GET['genre'] : '';
    // fungsi untuk memfilter data sesuai genre yang dipilih
    function filterByGenre($data, $genre)
    {
        if (empty($genre)) {
            return $data; // Jika tidak ada genre dipilih, kembalikan semua data
        }
        return array_filter($data, function ($item) use ($genre) {
            return $item['genre'] === $genre;
        });
    }
    $filteredData = filterByGenre($data, $selectedGenre);

    // Mengurutkan data berdasarkan pilihan pengguna
    if (isset($_GET['sort'])) {
        $sortKey = $_GET['sort'];
        // Misalnya, gunakan quickSort untuk pengurutan
     // Validasi input pengurutan dari form
        $validSortKeys = ['rating', 'popularitas', 'tahun_rilis'];
        if (in_array($sortKey, $validSortKeys)) {
            $data = quickSort($data, $sortKey);
        } else {
            echo "Kriteria pengurutan tidak valid.";
        }
    }

    // Jika tidak ada yang diurutkan
    if (empty($data)) {
        echo "<p>Tidak ada data untuk diurutkan.</p>";
    }
    ?>


    <?php
    echo "<h2>Daftar Film</h2>";
    echo "<table border='1'>";
    echo
    "<tr><th>Judul</th><th>Gambar</th><th>Genre</th><th>Popularitas</th><th>
    Rating</th><th>Tahun Rilis</th><th>Pemeran
    Utama</th></tr>";
    foreach ($data as $film) {
        echo "<tr>";
        echo "<td>" . $film["judul"] . "</td>";
        echo "<td><img src='images/" . htmlspecialchars($film["Gambar"]) .
            "' alt='" . htmlspecialchars($film["judul"]) .
            "' style='width:100px; height:auto;'></td>"; // Menampilkan gambar
        echo "<td>" . $film["genre"] . "</td>";
        echo "<td>" . $film["popularitas"] . "</td>";
        echo "<td>" . $film["rating"] . "</td>";
        echo "<td>" . $film["tahun_rilis"] . "</td>";
        echo "<td>" . $film["pemeran_utama"] . "</td>";
        echo "</tr>";
    }
    echo "</table>";
    ?>


    <div class="table-wrapper">
        <table>
            <p>Menampilkan hasil untuk genre: 
                <strong><?php echo
                !empty($selectedGenre) ? htmlspecialchars($selectedGenre)
                : 'Semua Genre'; ?></strong></p>
            <thead>
                <tr>
                    <th>Judul</th>
                    <th>Gambar</th>
                    <th>Rating</th>
                    <th>Popularitas</th>
                    <th>Tahun Rilis</th>
                </tr>
            </thead>
            <tbody>
                <?php if (!empty($filteredData)): ?>
                    <?php foreach ($filteredData as $item): ?>
                        <tr>
                            <td><?php echo
                                htmlspecialchars($item['judul']); ?></td>
                            <td>
                                <img src="images/<?php echo htmlspecialchars($item['Gambar']); ?>" 
                                style="width:80px;height:auto;">
                            </td>
                            <td><?php echo
                                htmlspecialchars($item['rating']); ?></td>
                            <td><?php echo
                                htmlspecialchars($item['popularitas']); ?></td>
                            <td><?php echo
                                htmlspecialchars($item['tahun_rilis']); ?></td>
                        </tr>
                    <?php endforeach; ?>
                <?php else: ?>
                    <tr>
                        <td colspan="4">Tidak ada data untuk
                            ditampilkan.</td>
                    </tr>
                <?php endif; ?>
            </tbody>
        </table>
    </div>
    <div class="table-container">
        <table border="1">
            <?php
            $kriteria = isset($_GET['sort']) ? $_GET['sort'] :
                'rating';
            $kriteriaText = ucfirst($kriteria);
            ?>
            <p>Menampilkan hasil yang diurutkan berdasarkan:
                <strong><?php echo $kriteriaText; ?></strong>
            </p>
            <thead>
                <tr>
                    <th>Judul</th>
                    <th>Gambar</th>
                    <th>Rating</th>
                    <th>Popularitas</th>
                    <th>Tahun Rilis</th>
                </tr>
            </thead>
            <tbody>
                <!-- Data akan ditampilkan di sini -->
                <?php if (!empty($data)): ?>
                    <?php foreach ($data as $item): ?>
                        <tr>
                            <td><?php echo
                                htmlspecialchars($item['judul']); ?></td>
                            <td>
                                <img src="images/<?php echo htmlspecialchars($item['Gambar']); ?>" 
                                style="width:80px;height:auto;">
                            </td>
                            <td><?php echo
                                htmlspecialchars($item['rating']); ?></td>
                            <td><?php echo
                                htmlspecialchars($item['popularitas']); ?></td>
                            <td><?php echo
                                htmlspecialchars($item['tahun_rilis']); ?></td>
                        </tr>
                    <?php endforeach; ?>
                <?php else: ?>
                    <tr>
                        <td colspan="4">Tidak ada data untuk
                            ditampilkan.</td>
                    </tr>
                <?php endif; ?>
            </tbody>
        </table>
    </div>
</body>

</html>

<?php
// fungsi mengembalikan array data yang telah diurutkan menggunakan quick sort
function quickSort($data, $key)
{
    if (count($data) < 2) {
        return $data;
    }
    $left = $right = [];
    $pivot = $data[0];
    for ($i = 1; $i < count($data); $i++) {
        if ($data[$i][$key] > $pivot[$key]) {
            $left[] = $data[$i];
        } else {
            $right[] = $data[$i];
        }
    }
    return array_merge(
        quickSort($left, $key),
        [$pivot],
        quickSort($right, $key)
    );
}
$data = quickSort($data, 'popularitas');

