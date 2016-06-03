package com.wiz.biografiatlit;


import android.os.Bundle;
import android.support.v4.app.Fragment;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.AdapterView;
import android.widget.ArrayAdapter;
import android.widget.ImageView;
import android.widget.Spinner;
import android.widget.TextView;

import butterknife.Bind;
import butterknife.ButterKnife;


public class BiodataAtlit extends Fragment implements  AdapterView.OnItemSelectedListener{

    private static final String[]nama = {"Susi Susanti", "Taufik Hidayat", "Chris John","Rudi Hartono","Alan Budikusuma"};
    private static final String[]bidang = {"Bulu Tangkis", "Bulu Tangkis", "Tinju","Bulu Tangkis","Bulu Tangkis"};

    @Bind(R.id.deskripsi)
    TextView deskripsi;
    @Bind(R.id.foto)
    ImageView foto;
    @Bind(R.id.spinner)
    Spinner spinner;

    public BiodataAtlit() {
        // Required empty public constructor
    }


    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        View view= inflater.inflate(R.layout.fragment_biodata_atlit, container, false);
        ButterKnife.bind(this, view);

        ArrayAdapter<String> adapter = new SpinnerAdapter(getContext(),
                android.R.layout.simple_spinner_item,this.nama,this.bidang);

        adapter.setDropDownViewResource(android.R.layout.simple_spinner_dropdown_item);
        spinner.setAdapter(adapter);
        spinner.setOnItemSelectedListener(this);

        selectArticle(0);

        return view;

    }

    @Override
    public void onItemSelected(AdapterView<?> parent, View view, int position, long id) {
        switch (position) {
            case 0:
                selectArticle(0);
                break;
            case 1:
                selectArticle(1);
                break;
            case 2:
                selectArticle(2);
                break;
            case 3:
                selectArticle(3);
                break;
            case 4:
                selectArticle(4);
                break;
        }
    }

    @Override
    public void onNothingSelected(AdapterView<?> parent) {

    }

    private void selectArticle(int position){
        switch (position){
            case 0:
                deskripsi.setText(
                        "Dia menikah dengan Alan Budikusuma, yang meraih medali emas bersamanya di Olimpiade Barcelona 1992. Selain itu, ia pernah juga meraih medali perunggu di Olimpiade Atlanta 1996 \n \n" +
                                "International Badminton Federation (sekarang Badminton World Federation) pada bulan Mei 2004 memberikan penghargaan Hall Of Fame kepada Susi Susanti. Pemain Indonesia lainnya yang memperoleh penghargaan Hall Of Fame yaitu Rudy Hartono Kurniawan, Dick Sudirman, Christian Hadinata, dan Liem Swie King."
                );
                foto.setImageResource(R.drawable.susi_susanti);
                break;
            case 1:
                deskripsi.setText(
                        "Taufik Hidayat (lahir di Bandung, Jawa Barat, 10 Agustus 1981, umur 27 tahun) adalah pemain bulutangkis tunggal putra dari Indonesia yang berasal dari klub SGS Elektrik Bandung dengan tinggi badan 176 cm.\n\n" +
                                "Putra pasangan Aris Haris dan Enok Dartilah ini adalah peraih medali emas untuk Indonesia pada Olimpiade Athena 2004 dengan mengalahkan Seung Mo Shon dari Korea Selatan di babak final. Pada 21 Agustus 2005, dia menjadi juara dunia dengan mengalahkan permain peringkat 1 dunia, Lin Dan di babak final, sehingga menjadi pemain tunggal putra pertama yang memegang gelar Kejuaraan Dunia Bulutangkis dan Olimpiade pada saat yang sama. Selain itu, ia juga sedang memegang gelar juara tunggal putra Asian Games (2002, 2006). Ia tampil di Olimpiade Beijing 2008, namun langsung kalah di pertandingan pertamanya, melawan Wong Choong Hann di babak kedua.\n\n" +
                                "Selain itu, dia juga telah enam kali menjuarai Indonesia Terbuka: 1999, 2000, 2002, 2003, 2004, dan 2006.\n\n" +
                                "Pengalaman lainnya antara lain pada Piala Thomas (2000, 2002, 2004, 2006 dan 2008) serta Piala Sudirman (1999, 2001, 2003 dan 2005)."
                );
                foto.setImageResource(R.drawable.taufik_hidayat);
                break;
            case 2:
                deskripsi.setText(
                        "Yohannes Christian John, atau lebih dikenal sebagai Chris John (lahir di Jakarta, 14 September 1979, umur 29 tahun) adalah seorang petinju Indonesia. Ia tercatat sebagai petinju Indonesia ketiga yang berhasil meraih gelar juara dunia, setelah Ellyas Pical dan Nico Thomas.");
                foto.setImageResource(R.drawable.chris_john);
                break;
            case 3:
                deskripsi.setText(
                        "Rudy Hartono Kurniawan (lahir di Surabaya, Jawa Timur, 18 Agustus 1949, umur 59 tahun) adalah seorang mantan pemain bulutangkis Indonesia. Ia pernah memenangkan kejuaraan dunia di tahun 1980, dan Kejuaraan All England selama 8 kali (7 diantaranya diraih secara berturut-turut) pada tahun 1960′an dan 1970′an." );
                foto.setImageResource(R.drawable.rudi_hartono);
                break;
            case 4:
                deskripsi.setText(
                        "Alan Budikusuma Wiratama (lahir di Surabaya, Jawa Timur, 29 Maret 1968, umur 41 tahun) adalah mantan pemain bulutangkis Indonesia yang meraih medali emas bulutangkis pada Olimpiade Barcelona 1992 dalam nomor tunggal putra. Ia pensiun dari dunia bulutangkis setelah Olimpiade Atlanta 1996.\n\n" +
                                "Alan menikah dengan Susi Susanti, yang juga memenangkan medali emas bulutangkis pada Olimpiade Barcelona.");
                foto.setImageResource(R.drawable.alan_budi_kusuma);
                break;
        }
    }
}
