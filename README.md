# camera-absensi
Fitur ini dibuat untuk absensi karyawan pada perusahaan.




# untuk mengatur camera resolusi.

 Webcam.set({
      width: 320,
      height: 240,

      image_format: 'jpeg',
      jpeg_quality: 90
    });
    
  # untuk menagkap file gambar dari camera
  
    Webcam.snap(function (data_uri) {
        // display results in page
        document.getElementById('results').innerHTML =
          '<img src="' + data_uri + '"/><input type="text" name="foto" value="' + data_uri + '" required/>';
      });
      
        # input disini decodebase 64 akan di convert melalui php agar menjandi PNG saat dikirimkan ke database.
       '<img src="' + data_uri + '"/><input type="text" name="foto" value="' + data_uri + '" required/>';
