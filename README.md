# Weve2050_Jewelry_Classifier

Jewelry SKU Classifier for Weve2050

## Goal

This project develops a machine learning model that identifies handmade jewelry SKUs from images when barcode information is unavailable.

Inventory management for handmade jewelry can be difficult because visually similar items may not have barcodes or easily searchable identifiers. The classifier is designed to help retail associates recognize the correct SKU quickly in situations such as:

- Updating inventory after checkout
- Looking up inventory while responding to customer inquiries
- Checking whether an SKU already exists when new stock arrives
- Identifying visually similar jewelry items that are difficult to distinguish manually

## Core Classification Features

The classifier is expected to:

- Identify the most likely SKU from an image
- Recommend the Top-3 most likely SKU candidates
- Allow the user to start a new SKU search

## Inventory Features

After an SKU is identified, the application may also allow the user to:

- View SKU information
- View current inventory
- Add a new SKU
- Update SKU information
- Increase or decrease inventory quantity
- Delete an SKU

## Proposed Machine Learning Approach

The initial baseline will use 1-NN on image features extracted from a pretrained vision model. The primary approach will use a pretrained image encoder with a linear classification layer to predict jewelry SKUs.

The project will evaluate both Top-1 and Top-3 classification accuracy, with particular attention to visually similar jewelry items and variations in lighting, angle, and reflections.
