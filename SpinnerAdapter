package com.wiz.biografiatlit;

import android.content.Context;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.ArrayAdapter;
import android.widget.TextView;

/**
 * Created by HP-G4 on 6/3/2016.
 */
public class SpinnerAdapter extends ArrayAdapter<String> {
    private String[] nama;
    private Context context;
    private String[] bidang;

    public SpinnerAdapter(Context context, int resourceId,
                              String[]nama,String[]bidang) {
        super(context, resourceId);
        this.nama = nama;
        this.context = context;
        this.bidang=bidang;
    }

    @Override
    public View getDropDownView(int position, View convertView,
                                ViewGroup parent) {
        return getCustomView(position, convertView, parent);
    }

    @Override
    public View getView(int position, View convertView, ViewGroup parent) {
        return getCustomView(position, convertView, parent);
    }

    @Override
    public int getCount() {
        return nama.length;
    }

    public View getCustomView(int position, View convertView, ViewGroup parent) {

        LayoutInflater inflater=(LayoutInflater) context.getSystemService(  Context.LAYOUT_INFLATER_SERVICE );
        View row=inflater.inflate(R.layout.custom_spinner, parent, false);
        TextView nama=(TextView)row.findViewById(R.id.sp_nama);
        TextView bidang=(TextView)row.findViewById(R.id.sp_bidang);

        nama.setText(this.nama[position]);
        bidang.setText(this.bidang[position]);

        /*if (position == 0) {//Special style for dropdown header
            nama.setTextColor(context.getResources().getColor(R.color.colorAccent));
        }*/

        return row;
    }
}
